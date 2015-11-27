
related link: https://forum.voltdb.com/showthread.php?49-Load-Balancing

We tried a few things - ultimately the servers will communicate with each other to decide which exact node should process a specific transaction, so bringing that logic the the client to try to preempt the decision will not help you as far as performance goes, or so minimally it certainly isn't worth the hair-splitting effort.
So... If you have a multi-node cluster, simply connect to all nodes and let the client library round-robin your requests (this is the answer to #1: the client library will simply round-robin requests to each node). Once the requests reaches a node, that node will communicate with the others to decide (based on K-safety and the partition target deduced from your partitioning key when you called the procedure), which specific sites (partitions on a specific node/list of nodes) will have to execute the transaction (that's the answer to #2)

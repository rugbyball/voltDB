> org.voltdb.client.ProcCallException:
Unexpected Ad Hoc Planning Error: java.lang.RuntimeException:
Error compiling query: org.voltdb.planner.PlanningErrorException:
Join of multiple partitioned tables has insufficient join criteria. <br />

If you ran into this kind of error <br />
"Join or union of multiple partitioned tables has insufficient join criteria.", <br />
VOLTDB assumes that the query is joined on multiple partitioned tables without sufficient join criteria. <br />
Currently, VOLTDB only support multiple partitioned tables join on their partitioned keys. <br />
This is because VOLTDB wants the multiple partitioned tables join only on each partition.  <br />

ref: https://forum.voltdb.com/showthread.php?1158-SQL-Insufficient-Join-Criteria


VoltPort died due to an unexpected exception
ref: https://forum.voltdb.com/showthread.php?35-NETWORK-VoltPort-died-due-to-an-unexpected-exception


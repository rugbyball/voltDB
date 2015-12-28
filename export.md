ERROR: Export is not supported in the community edition of VoltDB.
==============
FATAL: This process will exit. Please run VoltDB with a deployment file compatible with the community edition.
VoltDB has encountered an unrecoverable error and is exiting.
The log may contain additional information.


ERROR: [null]: Table with indexes configured as an export table
==============

failed: [vdb01] => {"changed": true, "cmd": ["/opt/voltdb/bin/voltdb", "compile", "/home/vagrant/cluster-test/db.sql", "--output=/home/vagrant/cluster-test/catalog.jar"], "delta": "0:00:01.843823", "end": "2015-12-28 16:36:34.454634", "rc": 1, "start": "2015-12-28 16:36:32.610811", "warnings": []}
stdout: WARN: [null]: The size of VARCHAR column TOTAL_SIZE in table OZ_APK_UPDATE_INFO greater than 262144 will be enforced as byte counts rather than UTF8 character counts. To eliminate this warning, specify "VARCHAR(1048576 BYTES)"
ERROR: While configuring export, table OZ_ROLE has indexes defined. Export tables can't have indexes (including primary keys).
ERROR: [null]: Table with indexes configured as an export table
------------------------------------------
Catalog compilation failed.
------------------------------------------

FATAL: all hosts have already failed -- aborting

# voltDB-errors
List voltDB errors, and some solutions for these error


### voltdb response status code
https://github.com/VoltDB/voltdb/blob/a796cf7b597cc180755736fade3e292e3b248808/tools/vmc_stats_emulator.py   

STATUS_STRINGS = {
  "VOLTDB_CONNECTION_LOST": -4,
  "VOLTDB_CONNECTION_TIMEOUT": -6,
  "VOLTDB_GRACEFUL_FAILURE": -2,
  "VOLTDB_OPERATIONAL_FAILURE": -9,
  "VOLTDB_RESPONSE_UNKNOWN": -7,
  "VOLTDB_SERVER_UNAVAILABLE": -5,
  "VOLTDB_SUCCESS": 1,
  "VOLTDB_TXN_RESTART": -8,
  "VOLTDB_UNEXPECTED_FAILURE": -3,
  "VOLTDB_UNINITIALIZED_APP_STATUS_CODE": -128,
  "VOLTDB_USER_ABORT": -1,
}

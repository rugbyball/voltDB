ant clean && ant -Djmemcheck=NO_MEMCHECK && ant dist  

client
===
/src/frontend/org/voltcore/network/VoltProtocolHandler.java  
//private static int MAX_MESSAGE_LENGTH = 52428800;  
private static int MAX_MESSAGE_LENGTH = 2097152000

server
===
/src/ee/storage/TempTableLimits.h  
TempTableLimits(int64_t memoryLimit = 1024 * 1024 * 100, int64_t logThreshold = -1)  

/src/ee/storage/TempTableLimits.cpp  

/src/ee/common/serializeio.cpp  
size_t maxAllocationSize = ((1024 * 1024 *50) - (1024 * 32));

/src/ee/voltdbipc.cpp  
#define MAX_MSG_SZ (1024*1024*10)  

src\frontend\org\voltdb  
2015.12.19 版本

ant clean && ant -Djmemcheck=NO_MEMCHECK && ant dist



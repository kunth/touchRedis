Background: 
get redis instance from sentinel, one master and one slave.
After set a key("mytestkey"), and always get the value("mytestvalue"); Each **3s** the program will get the value.

The log below have three phases:
1. the master is ok, as we can see "get keys result = mytestvalue"
2. then the master is kill, we see 20 "connect ECONNREFUSED"s
3. after that, we can see the result becomes OK. **Beware that 20 "in caller, get keys result = mytestvalue" comes out, which indicates that sentinel/ioredis won't drop the request during the master down and slave not promoted to master**

---------------in caller, get keys result = mytestvalue
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
---------------in caller, get keys result = mytestvalue
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
Error in redis-failover: rnode_33 had connection error
{ [Error: connect ECONNREFUSED]
  code: 'ECONNREFUSED',
  errno: 'ECONNREFUSED',
  syscall: 'connect' }
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
---------------in caller, get keys result = mytestvalue
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
---------------in caller, get keys result = mytestvalue
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
---------------in caller, get keys result = mytestvalue
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
---------------in caller, get keys result = mytestvalue
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
---------------in caller, get keys result = mytestvalue
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get
---------------in caller, get keys result = mytestvalue
[DEBUG INFO]in getClientByKey2, crc value = 134
[DEBUG INFO]in getClientByKey2, key = mytestkey, redisName = rnode_33
[DEBUG INFO]in clientProxy command = get

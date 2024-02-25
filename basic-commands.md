## cli

redis-cli
quit

## set + expire

SET name andiez
GET name
DEL name
EXISTS name
KEYS <pattern>
flushall -> clear
ttl name (return -1)
expire name 10 (min)
check ttl
setex name 10 andiez

## lists

lpush friends Andiez
lrange friends 0 -1
lpush friends Mike
rpush friends Pie
lpop friends (=Mike)
rpop friends (=Pie)

## sets

sadd hobbies "weight lifting" (return 1)
smembers hobbies
sadd hobbies "weight lifting" (return 0)
srem hobbies "weight lifting"

## hashes

hset wife name "Trang Beo"
hget wife name
hgetall wife (return 1,name - 2,Trang Beo)
hset wife age 18
hdel wife age
hexists wife name (return 1)
hexists wife age (return 0)
redis有五种类型:string,hash,list,set,zset(集合)
1.查看所有key
keys *
2.查看key类型
type 'key'


#=>h1;Hash:
存值:hmset 'key' field1 value1 field2 value2...
得到某一个值：hmget 'key' field
返回所有：hgetall 'key'
返回所有field：hkeys key
返回所有value：hvals key
删除：hdel key
设置key过期时间：expire key "秒数"
查看剩余时间

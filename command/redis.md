redis
===

redis终端操作

## 补充说明

**redis-cli命令** 进Redis交互模式

###  语法

```shell
redis(选项)(参数)
```

###  选项

```shell
-h：host；
-p：端口；
-c：集群模式；
```

###  参数

Redis语句：连接Redis后立即执行的语句。

## 实例

```shell
./redis-cli -h 10.17.7.239 -p 26380 -c
./redis-cli -h 10.17.7.239 -p 26380 -c SCAN 0 MATCH "TURN_TABEL_ORDER*" COUNT 10
./redis-cli -h 10.17.7.239 -p 26380 -c SCAN 0 MATCH "TURN_TABEL_ORDER*" COUNT 10 | wc -l
```

<!-- Linux命令行搜索引擎：https://jaywcjlove.github.io/linux-command/ -->

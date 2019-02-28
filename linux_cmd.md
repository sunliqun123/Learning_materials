
批量获取进程号并转换为一行数据

```shell
pgrep -l python3 | awk '{print 1}' | sed ':a;N;!ba;s/\n/ /g'
```

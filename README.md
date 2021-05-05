##### 情况报送
###### 使用
* 修改python主函数里的几个参数

###### crontab配置示例

```
30 6 * * * /usr/bin/sh /root/wut/qkbs.sh

cat /root/wut/qkbs.sh
logdir=/root/trash/qkbs.log && date >> $logdir && /usr/bin/python3 /root/wut/myqkbs.py >> $logdir

```

##### 原理分析
* 从server获取session
* 用这个session模拟那个绑定账号，这样这个session就是对应到账号的正确session了
* 进行情况报送

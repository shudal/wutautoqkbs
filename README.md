##### 情况报送
###### Authro: 王涵
###### 使用
* 修改python主函数里的几个参数

###### crontab配置示例

```
# 每天早上6.30执行脚本
30 6 * * * /usr/bin/sh /root/wut/qkbs.sh
```

##### 原理分析
* 从server获取session
* 用这个session模拟那个绑定账号，这样这个session就是对应到账号的正确session了
* 进行情况报送

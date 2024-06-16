### 从云平台上获取准确的时间

需要两个topic

![image-20240326150956735](文档中本地图片/image-20240326150956735.png)

我们需要定于NTP时钟同步响应，向NTP时钟同步请求发条指令

发布指令：

```
/ext/ntp/h2q0peMWuBX/aliyun_csdn_test/request
```

消息

```
{deviceSendTime:"111"}
```

订阅topic

```
/ext/ntp/h2q0peMWuBX/aliyun_csdn_test/response
```

发送消息后，订阅的发来时间

![image-20240326151902764](文档中本地图片/image-20240326151902764.png)

1711437534091转化（需要去掉后三位）

[时间戳(Unix timestamp)转换工具 - 在线工具 (tool.lu)](https://tool.lu/timestamp/)

![image-20240326152019968](文档中本地图片/image-20240326152019968.png)
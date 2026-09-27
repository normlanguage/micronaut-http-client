# Micronaut HTTP Client 示例

[English](README.md) | [简体中文](README.zh-CN.md)

[hello.norm](hello.norm) 创建 Micronaut 客户端，向仓库内的[本地模拟服务](local_server.py)发送同步 GET 请求、校验响应正文并关闭客户端。在仓库根目录启动模拟服务：

```sh
python samples/local_server.py
```

在另一个终端运行消费者：

```sh
norm run samples/hello.norm
```

程序输出 `Hello from Micronaut`。模拟服务仅监听 `127.0.0.1:18770`，按 Ctrl+C 停止。

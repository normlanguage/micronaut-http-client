# Micronaut HTTP Client sample

[English](README.md) | [简体中文](README.zh-CN.md)

[hello.norm](hello.norm) creates a Micronaut client, makes a blocking GET request to the included [local fixture](local_server.py), verifies the response body, and closes the client. From the repository root, start the fixture:

```sh
python samples/local_server.py
```

In another terminal, run the consumer:

```sh
norm run samples/hello.norm
```

It prints `Hello from Micronaut`. The fixture listens only on `127.0.0.1:18770`; stop it with Ctrl+C.

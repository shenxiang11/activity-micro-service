## Activity Micro Service

https://github.com/FE-star/activity-micro-service 的 GO 实现

## 重新编译 proto

进入 proto 目录，执行：

```bash
protoc --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative  activity-service.proto
```

## 重新生成执行文件

在项目根目录下，执行：

```bash
go build main.go
```

## 演示

### 正常请求

![](./screenshots/截屏2022-07-20%2018.01.13.png)

### 模拟错误

![](./screenshots/截屏2022-07-20%2018.01.21.png)
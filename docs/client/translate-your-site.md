---
sidebar_position: 2
---

# 执行节点开发
### .NetCore
可参考 [`src/OpenTask.Client` 
](https://github.com/SpringHgui/OpenTask/tree/f37696f51cf642a8dbf043fabb90568bdbf295e7/src/OpenTask.Client)

1. 安装nuget依赖 `dotnet add package OpenTask.Core`
2. 注册Handler
```
IHost host = Host.CreateDefaultBuilder(args)
.ConfigureServices((ctx, services) =>
{
    _ = services.AddOpenTaskWorker(ctx.Configuration.GetSection("OpenTaskWorker"), options =>
    {
        options.AddHandler<DemoJobHandler>();
        options.AddHandler<JobHandler>();
    });
})
.Build();

host.Run();
```
3. 配置文件
```
{
  "OpenTaskWorker": {
    "Addr": [ "127.0.0.1:1883" ],
    "AppName": "default"
  }
}
```
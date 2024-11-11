---
sidebar_position: 1
---

# 简介

[![Build status](https://github.com/SpringHgui/OpenTask/workflows/build/badge.svg)](https://github.com/SpringHgui/OpenTask/actions)
[![Nuget](https://img.shields.io/nuget/v/OpenTask.Core)](https://www.nuget.org/packages/OpenTask.Core/)

去中心设计的分布式任务调度平台，本项目不仅仅是创造一个新的轮子，旨在补充dotnet生态下分布式任务调度系统的空白，但本项目设计的并非只支持dotnet平台；

调度中心与执行器的通讯协议采用mqtt协议，方便多种语言的快速接入，调度中心采用去中心化设计，各个调度中心之间亦采用mqtt协议通讯；

调度中心自动进行任务分片，以平均每个调度节点的负载。

## 体验地址

http://opentask.run/  
账号：admin  
密码：OpenTask  


## 仓库地址

[Github](https://github.com/SpringHgui/OpenTask)

[Gitee](https://gitee.com/SpringHgui/OpenTask)

## 当前进度
⚠⚠⚠ 当前尚处于开发初期，请勿在重要的生产环境中使用。

- [x] web管理后台
- [x] cron任务
- [ ] 工作流（DAG）
- [ ] 固定周期任务
- [x] 调度中心集群部署
- [x] 调度中心自动分片
- [x] 任务重试
- [ ] 任务故障转移
- [ ] 进行中的任务支持取消
- [x] 失败告警

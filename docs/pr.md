---
sidebar_position: 99
---


# 贡献指南

开源项目的发展离不开社区的贡献，如果您在使用本项目中遇到问题或建议，欢迎多多提[issue](https://github.com/SpringHgui/OpenTask/issues)，对于符合大众的需求，我们将尽快进行完善。

如果您在使用中遇到了bug或者有bug的修改建议等，您可以直接创建[PR](https://github.com/SpringHgui/OpenTask/pulls)，感谢~

1. 开发数据库搭建
```
docker run -e MYSQL_DATABASE=open_task -e MYSQL_ROOT_PASSWORD=OPEN_TASK_!@# -p 3308:3306 --name=mysql8 -d registry.cn-hangzhou.aliyuncs.com/hgui/mysql:8.4.1
```
2. 安装vs2022
打开`OpenTask.sln`解决方案进行开发

3. 运行 `OpenTask.WebApi` 后端

3. 切到 `ui/vite-opentask` 运行前端项目

需要安装`node20`
```
npm i
npm run dev
```

默认用户名密码 admin/OpenTask

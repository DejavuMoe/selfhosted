# dejavu/selfhosted

这是一个用于记录和维护自托管应用的模板仓库，主要包含 **Docker Compose** 和 **Nginx 反向代理** 的配置模板，旨在帮助我快速部署常见的开源服务和私有化应用。

**本仓库适合用于：**

- 个人服务器/家庭服务器（HomeLab）快速部署
- VPS/VDS 环境下的一键式服务搭建
- 统一管理各类自托管服务的配置模板

## 结构说明

每个文件夹对应一个独立服务，通常包含：

- `docker-compose.yml`
- `.env` 示例文件
- `nginx.conf` 使用 Nginx 反向代理的配置模板
- 特殊部署说明及指南链接

## 收录服务

| 名称 | 说明 |
|------|------|
| [bark-server](barkserver/) | iOS Bark 推送服务的自托管服务器端实现 |
| blinko | 轻量级的个人笔记与知识管理工具 |
| cloudreve-pro | 支持多存储后端的私有云网盘系统 |
| gitea | 轻量级自托管 Git 代码托管平台 |
| hugo | 基于 Hugo 的静态网站构建与部署环境 |
| immich | 高性能的自托管照片与视频管理平台 |
| it-tolls | 常用 IT 工具集合的自托管服务 |
| nah.pet | 轻量级的自托管宠物类/个人展示站点 |
| ollama | 本地运行大语言模型的服务端环境 |
| plausible | 隐私友好的开源网站统计分析工具 |
| stirling-pdf | 开源的 PDF 处理与转换工具集 |
| twikoo | 静态网站评论系统的自托管后端 |
| uptime-kuma | 轻量级的服务状态监控面板 |
| wakapi | 开源的编码时间统计工具 |
| woodpecker-ci | 兼容 Drone 的轻量级持续集成系统 |

## 使用方式（简要）

1. 进入对应服务目录
2. 修改 `.env` 及 `docker-compose.yml` 里面的环境变量
3. 使用 Docker Compose 启动服务：
4. 修改 `nginx.conf` 里面的域名或反代信息
5. 启动服务

```bash
sudo docker compose up -d
```

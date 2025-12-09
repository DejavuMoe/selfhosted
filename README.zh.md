# dejavu/selfhosted

中文简体 | [English](README.md)

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

| 名称                                                         | 说明                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Bark Server](/dejavu/selfhosted/src/branch/master/bark-server) | iOS Bark 推送服务的自托管服务器端实现。                      |
| [Blinko](/dejavu/selfhosted/src/branch/master/blinko)        | 一款开源、自托管的个人 AI 笔记工具，优先保护隐私，使用 TypeScript 构建。 |
| [Cloudreve Pro](/dejavu/selfhosted/src/branch/master/cloudreve-pro) | 支持多存储后端的私有云网盘系统。                             |
| [Gitea](/dejavu/selfhosted/src/branch/master/gitea)          | 轻量级自托管 Git 代码托管平台。                              |
| [Hugo](/dejavu/selfhosted/src/branch/master/hugo)            | 基于 Hugo、Gitea 和 Woodpecker CI 的静态网站构建与部署环境。 |
| [immich](/dejavu/selfhosted/src/branch/master/immich)        | 高性能的自托管照片与视频管理平台。                           |
| [IT Tools](/dejavu/selfhosted/src/branch/master/it-tolls)    | 常用自托管 IT 工具集合。                                     |
| [nah.pet](/dejavu/selfhosted/src/branch/master/nah.pet)      | 重写短链接路径的另类方案——替代 TinyURL、YOURLS、Shlink。     |
| [Ollama](/dejavu/selfhosted/src/branch/master/ollama)        | 本地运行大语言模型的服务器环境。                             |
| [Plausible](/dejavu/selfhosted/src/branch/master/plausible)  | 简单易用且隐私友好的 Google Analytics 替代方案。             |
| [Stirling PDF](/dejavu/selfhosted/src/branch/master/stirling-pdf) | 可以在任何设备随时编辑 PDF 文件。                            |
| [Twikoo](/dejavu/selfhosted/src/branch/master/twikoo)        | 简单、安全且免费的评论系统。                                 |
| [Uptime Kuma](/dejavu/selfhosted/src/branch/master/uptime-kuma) | 精美的自托管服务监控工具。                                   |
| [Wakapi](/dejavu/selfhosted/src/branch/master/wakapi)        | 极简、自托管的 WakaTime 兼容后端，用于编码统计。             |
| [Woodpecker CI](/dejavu/selfhosted/src/branch/master/woodpecker-ci) | 简单而强大的 CI/CD 引擎，扩展性极佳。                        |
| [Forgejo](/dejavu/selfhosted/src/branch/master/forgejo)      | 一个自托管的轻量级软件锻造平台。安装简单，维护低，能完成任务。 |
| [Memos](/dejavu/selfhosted/src/branch/master/memos)          | 隐私优先的笔记服务，零遥测。没有跟踪，没有广告，没有订阅费。 |
| [OneDev](/dejavu/selfhosted/src/branch/master/onedev)        | 带有 CI/CD、看板和软件包的 Git 服务器。无缝集成。无与伦比的体验。 |
| [Pocket ID](/dejavu/selfhosted/src/branch/master/pocket-id)  | 一个简单易用的 OIDC 提供商，允许用户用通行密钥认证服务。     |
| [Tinyauth](/dejavu/selfhosted/src/branch/master/tinyauth)    | 保护你的应用，使用一个最简单的登录界面。                     |
| [n8n](/dejavu/selfhosted/src/branch/master/n8n)              | 具有原生 AI 功能的公平代码工作流自动化平台。                 |
| [Umami](/dejavu/selfhosted/src/branch/master/umami)          | 一个现代的、注重隐私的 Google Analytics 开源替代品。         |

## 使用方式（简要）

1. 进入对应服务目录
2. 修改 `.env` 及 `docker-compose.yml` 里面的环境变量
3. 使用 Docker Compose 启动服务：
4. 修改 `nginx.conf` 里面的域名或反代信息
5. 启动服务

```bash
sudo docker compose up -d
```

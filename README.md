# dejavu/selfhosted

English | [中文简体](README.zh.md)

This is a repository used to record and maintain self-hosted application templates. It mainly contains configuration templates for **Docker Compose** and **Nginx reverse proxy**, aiming to help quickly deploy common open-source services and private applications.

**This repository is suitable for:**

- Quick deployment on personal servers / HomeLab environments
- One-click service setup on VPS/VDS environments
- Centralized management of configuration templates for self-hosted services

## Structure

Each folder represents an independent service and usually contains:

- `docker-compose.yml`
- Example `.env` files
- `nginx.conf` templates for Nginx reverse proxy
- Special deployment instructions and guide links

## Included Services

| Name                                                         | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Bark Server](bark-server)                                   | Self-hosted server implementation for iOS Bark push service. |
| [Blinko](blinko)        | An open-source, self-hosted personal AI note tool prioritizing privacy, built using TypeScript. |
| [Cloudreve Pro](cloudreve-pro) | Private cloud storage system with support for multiple storage backends. |
| [Gitea](gitea)          | Lightweight self-hosted Git hosting platform.                |
| [Hugo](hugo)            | Static website build and deployment environment based on Hugo, Gitea and Woodpecker CI. |
| [immich](immich)        | High-performance self-hosted photo and video management platform. |
| [IT Tools](it-tools)    | Collection of commonly used self-hosted IT tools.            |
| [nah.pet](nah.pet)      | Rewriting paths with bad energy - An alternative to TinyURL, YOURLS, Shlink. |
| [Ollama](ollama)        | Server environment for running large language models locally. |
| [Plausible](plausible)  | Easy to use and privacy-friendly Google Analytics alternative. |
| [Stirling PDF](stirling-pdf) | Lets you edit PDFs on any device anywhere.                   |
| [Twikoo](twikoo)        | A simple, safe and free comment system.                      |
| [Uptime Kuma](uptime-kuma) | A fancy self-hosted monitoring tool.                         |
| [Wakapi](wakapi)        | A minimalist, self-hosted WakaTime-compatible backend for coding statistics. |
| [Woodpecker CI](woodpecker-ci) | A simple, yet powerful CI/CD engine with great extensibility. |
| [Forgejo](forgejo)      | A self-hosted lightweight software forge.Easy to install and low maintenance, it just does the job. |
| [Memos](memos)          | Privacy-first note-taking service with zero telemetry. No tracking, no ads, no subscription fees. |
| [OneDev](onedev)        | Git server with CI/CD, kanban, and packages. Seamless integration. Unparalleled experience. |
| [Pocket ID](pocket-id)  | A simple and easy-to-use OIDC provider that allows users to authenticate with their passkeys to your services. |
| [Tinyauth](tinyauth)    | The simplest way to protect your apps with a login screen.   |
| [n8n](n8n)              | Fair-code workflow automation platform with native AI capabilities. |
| [Umami](umami)          | A modern, privacy-focused analytics platform. An open-source alternative to Google Analytics. |

## Usage (Quick Guide)

1. Enter the corresponding service directory
2. Edit the environment variables in `.env` and `docker-compose.yml`
3. Use Docker Compose to start the service:
4. Edit the domain or reverse proxy settings in `nginx.conf`
5. Start the service

```bash
sudo docker compose up -d
```
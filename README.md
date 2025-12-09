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
| [bark-server](/dejavu/selfhosted/src/branch/master/bark-server) | Self-hosted server implementation for iOS Bark push service. |
| [blinko](/dejavu/selfhosted/src/branch/master/blinko)        | An open-source, self-hosted personal AI note tool prioritizing privacy, built using TypeScript. |
| [cloudreve-pro](/dejavu/selfhosted/src/branch/master/cloudreve-pro) | Private cloud storage system with support for multiple storage backends. |
| [gitea](/dejavu/selfhosted/src/branch/master/gitea)          | Lightweight self-hosted Git hosting platform.                |
| [hugo](/dejavu/selfhosted/src/branch/master/hugo)            | Static website build and deployment environment based on Hugo, Gitea and Woodpecker CI. |
| [immich](/dejavu/selfhosted/src/branch/master/immich)        | High-performance self-hosted photo and video management platform. |
| [it-tolls](/dejavu/selfhosted/src/branch/master/it-tolls)    | Collection of commonly used self-hosted IT tools.            |
| [nah.pet](/dejavu/selfhosted/src/branch/master/nah.pet)      | Rewriting paths with bad energy - An alternative to TinyURL, YOURLS, Shlink. |
| [ollama](/dejavu/selfhosted/src/branch/master/ollama)        | Server environment for running large language models locally. |
| [plausible](/dejavu/selfhosted/src/branch/master/plausible)  | Easy to use and privacy-friendly Google Analytics alternative. |
| [stirling-pdf](/dejavu/selfhosted/src/branch/master/stirling-pdf) | Lets you edit PDFs on any device anywhere.                   |
| [twikoo](/dejavu/selfhosted/src/branch/master/twikoo)        | A simple, safe and free comment system.                      |
| [uptime-kuma](/dejavu/selfhosted/src/branch/master/uptime-kuma) | A fancy self-hosted monitoring tool.                         |
| [wakapi](/dejavu/selfhosted/src/branch/master/wakapi)        | A minimalist, self-hosted WakaTime-compatible backend for coding statistics. |
| [woodpecker-ci](/dejavu/selfhosted/src/branch/master/woodpecker-ci) | A simple, yet powerful CI/CD engine with great extensibility. |
| [forgejo](/dejavu/selfhosted/src/branch/master/forgejo)      | A self-hosted lightweight software forge.Easy to install and low maintenance, it just does the job. |
| [memos](/dejavu/selfhosted/src/branch/master/memos)          | Privacy-first note-taking service with zero telemetry. No tracking, no ads, no subscription fees. |
| [onedev](/dejavu/selfhosted/src/branch/master/onedev)        | Git server with CI/CD, kanban, and packages. Seamless integration. Unparalleled experience. |
| [pocket-id](/dejavu/selfhosted/src/branch/master/pocket-id)  | A simple and easy-to-use OIDC provider that allows users to authenticate with their passkeys to your services. |
| [tinyauth](/dejavu/selfhosted/src/branch/master/tinyauth)    | The simplest way to protect your apps with a login screen.   |

## Usage (Quick Guide)

1. Enter the corresponding service directory
2. Edit the environment variables in `.env` and `docker-compose.yml`
3. Use Docker Compose to start the service:
4. Edit the domain or reverse proxy settings in `nginx.conf`
5. Start the service

```bash
sudo docker compose up -d
```
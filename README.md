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

| Name | Description |
|------|-------------|
| [bark-server](barkserver/) | Self-hosted server implementation for iOS Bark push service |
| blinko | Lightweight personal notes and knowledge management tool |
| cloudreve-pro | Private cloud storage system with support for multiple storage backends |
| gitea | Lightweight self-hosted Git hosting platform |
| hugo | Static website build and deployment environment based on Hugo |
| immich | High-performance self-hosted photo and video management platform |
| it-tolls | Collection of commonly used self-hosted IT tools |
| nah.pet | Lightweight self-hosted pet-themed / personal showcase website |
| ollama | Server environment for running large language models locally |
| plausible | Privacy-friendly open-source web analytics tool |
| stirling-pdf | Open-source PDF processing and conversion toolkit |
| twikoo | Self-hosted backend for static website comment system |
| uptime-kuma | Lightweight uptime and service monitoring dashboard |
| wakapi | Open-source coding activity tracking tool |
| woodpecker-ci | Lightweight continuous integration system compatible with Drone |

## Usage (Quick Guide)

1. Enter the corresponding service directory
2. Edit the environment variables in `.env` and `docker-compose.yml`
3. Use Docker Compose to start the service:
4. Edit the domain or reverse proxy settings in `nginx.conf`
5. Start the service

```bash
sudo docker compose up -d
```
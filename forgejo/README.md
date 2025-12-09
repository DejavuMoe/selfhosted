## Forgejo

>Forgejo is a self-hosted lightweight software forge.Easy to install and low maintenance, it just does the job.

- Source Code: https://codeberg.org/forgejo/forgejo
- Website: https://forgejo.org/
- Docs: https://forgejo.org/docs/latest/

## Two compose templates are provided here:

- [Forgejo](docker-compose.yml)
- [Forgejo with Woodpecker CI](forgejo-woodpecker-ci-compose.yml)

## Two nginx.conf templates are provided here:

- [Forgejo](nginx.conf)
- [Forgejo with Woodpecker CI](../woodpecker-ci/nginx.conf)

## Guide

- [Docker 部署 Forgejo 个人代码托管服务](https://blog.dejavu.moe/posts/docker-install-gitea-with-nginx-and-cloudflared/)
- [自托管 Forgejo 集成 Woodpecker CI/CD](https://blog.dejavu.moe/posts/selfhosted-gitea-ci-with-woodpecker/)
- [Woodpecker CI 和 Forgejo 实现 Hugo 自动部署](https://blog.dejavu.moe/posts/build-hugo-site-with-gitea-and-woodpecker-ci/)
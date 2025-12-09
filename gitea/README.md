## Gitea

>Painless self-hosted all-in-one software development service, including Git hosting, code review, team collaboration, package registry and CI/CD.

- Source Code: https://github.com/go-gitea/gitea
- Website: https://about.gitea.com/
- Docs: https://docs.gitea.com/

## Two compose templates are provided here:

- [Gitea](docker-compose.yml)
- [Gitea with Woodpecker CI](gitea-with-woodpecker-ci-compose.yml)

## Two nginx.conf templates are provided here:

- [Gitea](nginx.conf)
- [Gitea with Woodpecker CI](../woodpecker-ci/nginx.conf)

## Guide

- [Docker 部署 Gitea 个人代码托管服务](https://blog.dejavu.moe/posts/docker-install-gitea-with-nginx-and-cloudflared/)
- [自托管 Gitea 集成 Woodpecker CI/CD](https://blog.dejavu.moe/posts/selfhosted-gitea-ci-with-woodpecker/)
- [Woodpecker CI 和 Gitea 实现 Hugo 自动部署](https://blog.dejavu.moe/posts/build-hugo-site-with-gitea-and-woodpecker-ci/)
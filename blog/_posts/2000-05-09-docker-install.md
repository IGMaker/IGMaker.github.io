---
layout: post
title: Docker Install 및 Jekyll 환경 설정
sitemap: false
description: >
    Docker 설치과정 및 Jekyll 이미지 생성, 환경설정
hide_description: false
hide_last_modified: true
---

![](../../assets/img/blogs/docker_logo.png){:width="600"}

## Docker 설치

- Docker Server 설치
 
```sh
brew install --cask docker
```

![](../../assets/img/blogs/docker_server_install.png)

- Docker Client 설치

```sh
brew install docker
```

![](../../assets/img/blogs/docker_client_install.png)

도커 서버를 실행한다.

![](../../assets/img/blogs/docker-server-running.png)

### Jekyll 이미지 다운로드

```sh
docker pull jekyll/jekyll
```

### Jekyll 이미지 실행

```sh
docker run --rm -it --platform=linux/amd64/v8 jekyll/jekyll
```
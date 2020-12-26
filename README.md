<!-- Title & Logo -->
<h1 align="center">Docker-Nginx-Proxy</h1>

<!-- tag & links (Version\Lang\Package) -->
<p align="center">
    <img src="https://img.shields.io/badge/docker-lastest-4795e6" alt="docker" />
    <img src="https://img.shields.io/badge/nginx-lastest-4a9d59" alt="nginx" />
</p>
<p align="center">
    Source：<a href="https://github.com/evilz0212/docker-sample-project">Github</a>
	<!-- Demo：<a href="https://evilz0212.github.io/docker-sample-project/">Git Pages</a> -->
<p>

<!-- Overview (Preview\Purpose\Description) -->
![Docker-Nginx-Proxy](./public/preview.png)

## Overview
> 同域名下使用路徑判斷代理到前端或後端 ( /api ) 
#### Target
1. 使用 Docker 容器分離前後端專案環境
2. Nginx-proxy 連結 Docker Network 代理前後端服務

#### Detail
-  Docker：multi 建置設定
-  Docker-compose：自訂容器 networks 設定
-  Nginx：proxy_pass(docker container)

<!-- Get started (Install\Step) -->
## Get started (dev)
#### Installation
set hosts
```
hosts -> 127.0.0.1 docker.example.com
```
run docker-server
```
cd frontend-web && docker-compose up -d
```
```
cd backend-web && docker-compose up -d
```
```
cd nginx-proxy && docker-compose up -d
```
#### Note
links
```
FE: https://docker.example.com
```
```
BE: https://docker.example.com/api
```

<!-- Partner -->

<!-- License -->


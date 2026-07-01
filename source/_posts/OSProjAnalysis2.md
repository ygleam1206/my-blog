---
title: 开源项目分析（二）
date: 2026-07-01 21:46:37
categories:
  - 开源项目分析
tags:
  - 项目分析流程
  - 学习笔记
---

# 开源项目分析流程

```text
拿到 GitHub 项目
        │
        ▼
① README.md（项目介绍、运行方式）
        │
        ▼
② LICENSE（开源协议）
        │
        ▼
③ 判断技术栈
        │
        ├── 使用什么语言？
        ├── 使用什么框架？
        └── 使用什么运行环境？
        │
        ▼
④ 找项目配置文件
        │
        ├── Java → pom.xml
        ├── JavaScript → package.json
        └── Python → pyproject.toml / requirements.txt
        │
        ▼
⑤ 安装依赖
        │
        ├── npm install
        ├── mvn install
        └── pip install -r requirements.txt
        │
        ▼
⑥ 启动项目
        │
        ├── npm run serve / npm run dev
        ├── mvn spring-boot:run
        └── python main.py
        │
        ▼
⑦ 体验项目功能
        │
        ▼
⑧ 阅读源码
```

---

# 不同语言对应关系

| 语言 | 运行环境 | 项目配置 | 主流框架 |
|------|----------|----------|----------|
| Java | JVM | pom.xml | Spring Boot |
| JavaScript | Node.js | package.json | Vue / React / Express |
| Python | Python解释器 | pyproject.toml / requirements.txt | Django、FastAPI |
| Go | Go Runtime | go.mod | Gin |
| C# | .NET Runtime | .csproj | ASP.NET Core |
| PHP | PHP解释器 | composer.json | Laravel |

---

# 前后端技术栈关系

```text
浏览器
    │
    ▼
前端（Vue / React）
    │
HTTP
    │
    ▼
后端（Spring Boot / Express / Django）
    │
    ▼
数据库（MySQL / PostgreSQL / Redis）
```

---

# JavaScript 技术栈

```text
JavaScript（语言）
        │
        ▼
Node.js（运行环境）
        │
        ├── node（运行 JS）
        └── npm（依赖管理）
        │
        ▼
package.json（项目配置）
        │
        ▼
Vue / React（前端框架）
Express（后端框架）
```

---

# Java 技术栈

```text
Java（语言）
      │
      ▼
JVM（运行环境）
      │
      ▼
pom.xml（项目配置）
      │
      ▼
Spring Boot（后端框架）
```

---

# Python 技术栈

```text
Python（语言）
      │
      ▼
Python解释器（运行环境）
      │
      ▼
pyproject.toml / requirements.txt
      │
      ▼
Django / FastAPI
```

---

# Node.js 项目常见文件

| 文件 | 作用 |
|------|------|
| README.md | 项目说明 |
| LICENSE | 开源协议 |
| package.json | 项目配置、依赖、启动命令 |
| package-lock.json | 锁定依赖版本 |
| src | 源代码 |
| public | 静态资源 |
| node_modules | 安装的依赖 |

---

# package.json 重点关注

## scripts

运行命令：

```bash
npm run serve
npm run dev
npm run build
```

---

## dependencies

项目运行依赖。

---

## devDependencies

开发依赖。

---

# npm 常用命令

```bash
npm install
npm run serve
npm run dev
npm run build
```

---

# 终端常用命令

```bash
pwd
ls
cd
cd ..
cd ~
```
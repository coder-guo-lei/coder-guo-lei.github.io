---
title: 智教 AI+ 智能教学平台
date: 2026-06-12 20:00:00
categories:
  - 项目经验
tags:
  - Vue3
  - AI
  - SSE
  - RAG
  - Markdown
index_img: /img/default.png
---

## 项目介绍

智教 AI+ 智能教学是一套面向高职院校的 AI 智能教学与内容生产平台，集 **AI 对话、知识库问答、智能体协作、AI 撰写、报告生成、文档管理**等能力于一体。平台支持 SSE 流式输出、RAG 知识库检索增强、Markdown 富文本渲染、多栏协同编辑等功能。

**应用技术**：`Vue3` `Vite` `Pinia` `SSE` `KaTeX` `Mermaid` `Vditor` `Axios` `WebSocket` `Markdown-it`

---

## 我的职责

作为核心前端开发，独立负责 AI 平台前端整体架构设计与核心模块开发：

### 架构搭建
- 完成 **Vue3 + TypeScript** 工程化体系搭建，制定目录规范、组件规范与状态管理方案

### AI 流式对话
- 基于 **Fetch + ReadableStream** 实现 AI 大模型 SSE 流式对话能力
- 支持 JSON 数据流解析、内容增量渲染、思维链（reasoning_content）展示、异常中断恢复

### 通用架构设计
- 抽象通用 AI 聊天架构，设计 **baseChatStore** 与页面级 Store 工厂
- 实现消息列表、会话状态、知识库绑定、上下文管理等能力复用

### 富文本渲染
- 集成 **Markdown-it、KaTeX、Mermaid、代码高亮**等能力
- 实现 AI 回复内容中的公式渲染、流程图生成、代码块展示

### RAG 知识库
- 开发 RAG 知识库模块，支持知识库上传、标签筛选、文件管理、内容预览
- 支持基于私有知识库的智能问答与内容检索

### 智能体系统
- 实现智能体（Agent）广场、AI 撰写、方案生成等业务模块
- 支持模板化生成、流式输出、目录自动生成、内容续写

### 性能优化
- 通过虚拟滚动、增量渲染、路由懒加载、静态资源压缩等方案降低页面卡顿

### 工程化建设
- 统一 **ESLint + Prettier + Husky + Commitlint** 开发规范

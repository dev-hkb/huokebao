# 获客宝 — 你的24小时获客搭档

抖音获客自动化桌面工具，基于 Node.js 全栈 + Electron 33 客户端。

[![Download](https://img.shields.io/badge/下载-最新版本-4f46e5)](https://github.com/dev-hkb/huokebao/releases)
[![Platform](https://img.shields.io/badge/平台-macOS%20|%20Windows-lightgrey)]()
[![License](https://img.shields.io/badge/许可-商业软件-blue)]()
[![Website](https://img.shields.io/badge/官网-dev--hkb.github.io%2Fhuokebao-green)](https://dev-hkb.github.io/huokebao/)

---

## 亮点功能

### 🎯 自动化获客引擎
- **可视化策略配置** — 搜索关键词 + 目标用户画像 + 互动策略，图形化编排
- **7×24 无人值守** — 定时启动、智能休眠、异常自恢复
- **多账号并行** — 账号池管理，轮流切换避免风控

### 📹 视频评论区截流
- 监控目标账号新发视频，**秒级响应**，第一时间抢占评论区
- 自动匹配评论模板，支持变量替换（昵称、时间、关键词）
- 已评论视频自动记录，避免重复

### 📡 直播监控
- **WebSocket + Protobuf** 实时接入抖音直播间
- 弹幕流、礼物榜、观众列表实时采集
- 高价值用户自动标记入库

### 💬 DM 私信触达
- 批量发送自定义模板私信
- **ECDSA 签名协议**，兼容抖音最新接口
- 发送状态追踪 + Webhook 回调通知

### 🤖 智能验证码识别
- 深度学习 OCR 引擎识别，毫秒级响应
- 滑块验证码、点选验证码全自动识别
- 识别失败自动重试 + 策略降级

### 🛡️ 企业级反检测
- Chromium 浏览器指纹混淆引擎
- WebRTC 防泄露、Canvas 指纹随机化、FontFace 防护
- 全面通过主流自动化检测平台

### 📊 线索管理与转化
- 全量采集数据沉淀到本地 SQLite 数据库
- 多维筛选：来源、互动类型、时间范围、关键词
- 一键导出 Excel，支持自定义字段

### 🔄 智能自动更新
- 基于 GitHub Releases 的增量更新
- 启动自动检测新版本，应用内下载 + 安装
- 进度条 + 发布说明弹窗，透明升级

### 🔐 授权与安全
- 硬件绑定设备授权（macOS / Windows UUID）
- 24 小时免费试用
- SQLCipher 加密本地数据库

---

## 技术架构

| 层 | 技术 |
|---|------|
| 前端 | Vue 3 + Element Plus + ECharts |
| 桌面壳 | Electron 33 (Node.js 22) |
| 存储 | SQLite (better-sqlite3 + Drizzle ORM) |
| 加密 | SQLCipher (硬件 UUID 密钥) |
| 签名 | ECDSA (dycast getAbogus) |
| 验证码 | 深度学习 OCR (滑块识别) |
| 反检测 | Chromium 指纹混淆引擎 |
| 更新 | electron-updater (GitHub Releases) |

---

## 安装

前往 [Releases](https://github.com/dev-hkb/huokebao/releases) 下载对应平台安装包：

- **macOS**（Apple Silicon / Intel）：下载 `.dmg`，拖入 Applications
- **Windows**（x64）：下载 `.exe`，双击安装

首次启动自动获得 24 小时免费试用。

---

## 官网

https://dev-hkb.github.io/huokebao/

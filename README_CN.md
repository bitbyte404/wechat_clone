# 微信 Clone

[English](README.md) | [中文](README_CN.md)

一个使用 Flutter 构建的微信 UI 克隆项目，实现了微信的核心界面和功能。

## 功能特性

- 🏠 **首页** - 聊天列表，显示最近会话
- 👥 **通讯录** - 联系人列表，按字母分组
- 🔍 **发现** - 朋友圈、扫一扫、搜一搜、看一看、游戏、小程序
- 👤 **我** - 个人信息页面，包含设置和服务
- 💬 **聊天** - 实时消息界面，带消息气泡
- 🔐 **登录/注册** - 手机号登录和注册流程
- 💾 **本地存储** - 使用 SQLite 数据库进行数据持久化

## 截图预览

应用包含以下主要页面：

| 聊天列表 | 通讯录 | 发现 | 我 |
|---------|-------|------|-----|
| 消息列表 | 好友列表 | 功能入口 | 个人信息 |

## 技术栈

- **框架**: Flutter 3.5+
- **语言**: Dart
- **数据库**: SQLite (sqflite)
- **状态管理**: StatefulWidget
- **资源生成**: flutter_gen
- **本地存储**: shared_preferences

## 环境要求

- Flutter SDK ^3.5.4
- Dart SDK ^3.5.4
- Android Studio / VS Code
- Android SDK / Xcode（iOS 开发）

## 安装步骤

1. 克隆仓库
```bash
git clone https://github.com/bitbyte404/wechat_clone.git
cd wechat_clone
```

2. 安装依赖
```bash
flutter pub get
```

3. 生成资源文件
```bash
flutter pub run build_runner build
```

4. 运行应用
```bash
flutter run
```

## 项目结构

```
lib/
├── db/                 # 数据库辅助类
├── demo/               # 演示组件
├── gen/                # 生成的资源
├── generated/          # 生成的代码
├── mock/               # 模拟数据
├── models/             # 数据模型
├── ui/
│   ├── custom_widget/  # 可复用组件
│   └── pages/          # 应用页面
├── utls/               # 工具函数
├── value/              # 常量（颜色、尺寸）
└── main.dart           # 入口文件
```

## 主要页面

- `page_home.dart` - 主页标签导航
- `page_wechat.dart` - 聊天列表页
- `page_contact.dart` - 通讯录页面
- `page_find.dart` - 发现页面
- `page_mine.dart` - 个人信息页面
- `page_chat.dart` - 聊天对话页面
- `page_login.dart` - 登录页面
- `page_register.dart` - 注册页面

## 贡献

欢迎贡献代码！请随时提交 Pull Request。

## 许可证

本项目仅供学习和研究目的。微信是腾讯公司的商标。

## 致谢

- Flutter 团队提供的优秀框架
- 微信提供的 UI 设计灵感

# WeChat Clone

[English](README.md) | [中文](README_CN.md)

A WeChat UI clone built with Flutter, implementing the core interface and features of WeChat.

## Features

- 🏠 **Home Page** - Chat list with recent conversations
- 👥 **Contacts** - Contact list with alphabetical grouping
- 🔍 **Discover** - Moments, Scan, Search, Top Stories, Games, Mini Programs
- 👤 **Me** - Profile page with settings and services
- 💬 **Chat** - Real-time messaging interface with message bubbles
- 🔐 **Login/Register** - Phone number login and registration flow
- 💾 **Local Storage** - SQLite database for persistent data storage

## Screenshots

The app includes the following main pages:

| Chat List | Contacts | Discover | Profile |
|-----------|----------|----------|---------|
| Message list | Friend list | Feature entries | User profile |

## Tech Stack

- **Framework**: Flutter 3.5+
- **Language**: Dart
- **Database**: SQLite (sqflite)
- **State Management**: StatefulWidget
- **Asset Generation**: flutter_gen
- **Local Storage**: shared_preferences

## Prerequisites

- Flutter SDK ^3.5.4
- Dart SDK ^3.5.4
- Android Studio / VS Code
- Android SDK / Xcode (for iOS)

## Installation

1. Clone the repository
```bash
git clone https://github.com/bitbyte404/wechat_clone.git
cd wechat_clone
```

2. Install dependencies
```bash
flutter pub get
```

3. Generate assets
```bash
flutter pub run build_runner build
```

4. Run the app
```bash
flutter run
```

## Project Structure

```
lib/
├── db/                 # Database helpers
├── demo/               # Demo components
├── gen/                # Generated assets
├── generated/          # Generated code
├── mock/               # Mock data
├── models/             # Data models
├── ui/
│   ├── custom_widget/  # Reusable widgets
│   └── pages/          # App pages
├── utls/               # Utility functions
├── value/              # Constants (colors, sizes)
└── main.dart           # Entry point
```

## Main Pages

- `page_home.dart` - Main tab navigation
- `page_wechat.dart` - Chat list page
- `page_contact.dart` - Contacts page
- `page_find.dart` - Discover page
- `page_mine.dart` - Profile page
- `page_chat.dart` - Chat conversation page
- `page_login.dart` - Login page
- `page_register.dart` - Registration page

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is for educational purposes only. WeChat is a trademark of Tencent.

## Acknowledgments

- Flutter team for the amazing framework
- WeChat for the UI inspiration

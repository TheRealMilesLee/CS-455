# CS-455 Project README
## Project Overview
The CS-455 project consists of two Android applications designed for SMS-related functionality:
- **NumVerify**: A phone number verification application
- **ReadSMS**: An SMS message reading application
Both applications follow standard Android project structure with Java-based implementation and resource files for UI components.
## Installation
1. Clone the repository
2. Open the project in Android Studio
3. Ensure Gradle wrapper is properly configured
4. Sync project with Gradle files
## Usage
### NumVerify
1. Navigate to `AndroidSMS/NumVerify`
2. Build and run the application
3. Implement phone number verification logic through the provided Java classes
### ReadSMS
1. Navigate to `ReadSMS`
2. Build and run the application
3. Utilize SMS reading functionality through the main application logic
## File Structure
.
├── AndroidSMS
│   └── NumVerify
│       ├── .idea
│       ├── app
│       │   ├── androidTest
│       │   │   └── java
│       │   │       └── com
│       │   │           └── example
│       │   │               └── numverify
│       │   ├── main
│       │   │   ├── java
│       │   │   │   └── com
│       │   │   │       └── example
│       │   │   │           └── numverify
│       │   │   ├── res
│       │   │   │   ├── drawable
│       │   │   │   ├── drawable-v24
│       │   │   │   ├── layout
│       │   │   │   ├── mipmap-anydpi-v26
│       │   │   │   ├── mipmap-anydpi-v33
│       │   │   │   ├── mipmap-hdpi
│       │   │   │   ├── mipmap-mdpi
│       │   │   │   ├── mipmap-xhdpi
│       │   │   │   ├── mipmap-xxhdpi
│       │   │   │   ├── mipmap-xxxhdpi
│       │   │   │   ├── values
│       │   │   │   ├── values-night
│       │   │   │   └── xml
│       │   │   └── test
│       │   │       └── java
│       │   │           └── com
│       │   │               └── example
│       │   │                   └── numverify
│       │   └── test
│       │       └── java
│       │           └── com
│       │               └── example
│       │                   └── numverify
│       ├── gradle
│       └── wrapper
├── ReadSMS
│   ├── .idea
│   │   └── codeStyles
│   ├── app
│   │   ├── androidTest
│   │   │   └── java
│   │   │       └── com
│   │   │           └── example
│   │   │               └── readsms
│   │   ├── main
│   │   │   ├── java
│   │   │   │   └── com
│   │   │   │       └── example
│   │   │   │           └── readsms
│   │   │   ├── res
│   │   │   │   ├── drawable
│   │   │   │   ├── drawable-v24
│   │   │   │   ├── layout
│   │   │   │   ├── mipmap-anydpi-v26
│   │   │   │   ├── mipmap-anydpi-v33
│   │   │   │   ├── mipmap-hdpi
│   │   │   │   ├── mipmap-mdpi
│   │   │   │   ├── mipmap-xhdpi
│   │   │   │   ├── mipmap-xxhdpi
│   │   │   │   ├── mipmap-xxxhdpi
│   │   │   │   ├── values
│   │   │   │   ├── values-night
│   │   │   │   └── xml
│   │   │   └── test
│   │   │       └── java
│   │   │           └── com
│   │   │               └── example
│   │   │                   └── readsms
│   │   └── test
│   │       └── java
│   │           └── com
│   │               └── example
│   │                   └── readsms
│   └── gradle
│       └── wrapper
├── .gitignore
├── LICENSE
├── .gitattributes
├── .hgignore
├── .hgtags
├── .idea
├── .travis.yml
├── build.gradle
├── gradle
│   └── wrapper
├── settings.gradle
└── README.md
## Dependencies
- Android SDK (version specified in `build.gradle`)
- Gradle wrapper (version specified in `gradle-wrapper.properties`)
- Android Studio (for project development)
## Contribution Guidelines
- Report issues through the project's issue tracker
- Propose new features or improvements
- Submit pull requests with clear descriptions
- Follow the project's coding conventions and style guide
## License
This project is licensed under the terms of the [LICENSE](LICENSE) file.

---

## 中文版本

# CS-455
## 项目简介
## 项目结构说明
.
├── AndroidSMS
│   ├── NumVerify
│   │   ├── .idea
│   │   ├── app
│   │   │   ├── src
│   │   │   │   ├── androidTest
│   │   │   │   │   └── java
│   │   │   │   ├── main
│   │   │   │   │   ├── java
│   │   │   │   │   └── res
│   │   │   │   └── test
│   │   │   └── gradle
│   │   └── wrapper
│   └── ReadSMS
│       ├── .idea
│       │   └── codeStyles
│       ├── app
│       │   ├── src
│       │   │   ├── androidTest
│       │   │   │   └── java
│       │   │   ├── main
│       │   │   │   ├── java
│       │   │   │   └── res
│       │   │   └── test
│       │   └── gradle
│       └── wrapper
├── .gitignore
├── LICENSE
└── Submission
## 安装方式
1. 通过 Android Studio 打开项目目录
2. 使用 Gradle 构建工具执行 `./gradlew build` 命令
## 使用方法
### NumVerify 模块
- 实现手机号码验证功能，需通过用户输入接口获取待验证号码
- 通过 API 调用或本地规则校验号码格式有效性
### ReadSMS 模块
- 实现短信内容读取功能，需获取短信数据库读取权限
- 支持按时间范围、联系人等条件筛选短信记录
## 依赖项
- Android SDK 基础库
- Android Testing Support Library
- Android Gradle 插件
## 开发与贡献指南
### 贡献规范
1. 请使用 Java 语言进行开发
2. 遵循 Android 开发者指南的编码规范
3. 新增功能需配套单元测试
### 开发建议
- NumVerify 模块建议扩展号码格式校验规则
- ReadSMS 模块建议增加短信内容过滤功能
- 请确保所有 API 调用符合 Android 权限模型
### 测试要求
- 必须通过 Android 单元测试框架验证核心功能
- 短信读取功能需在模拟器或物理设备上验证

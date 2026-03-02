# LumiNya - Android WebView App

## 项目信息
- **应用名称**: LumiNya
- **包名**: cc.luminya.lumiapp
- **网站地址**: https://luminya.cc
- **最低Android版本**: API 26

## 构建说明

### 方法1: 使用 Android Studio
1. 打开 Android Studio
2. 选择 "Open an existing Android Studio project"
3. 选择解压后的项目文件夹
4. 等待 Gradle 同步完成
5. 点击 Build > Generate Signed Bundle / APK
6. 选择 APK，然后创建或选择签名密钥
7. 选择 release 构建类型
8. 点击 Finish 生成 APK

### 方法2: 使用命令行
```bash
# 进入项目目录
cd LumiNya

# 生成 debug APK
./gradlew assembleDebug

# 生成 release APK (需要配置签名)
./gradlew assembleRelease
```

生成的 APK 位于: `app/build/outputs/apk/`

## 功能配置
- 屏幕方向: portrait
- 全屏模式: false
- 文件上传: true
- 位置权限: true
- 相机权限: true
- 退出确认: true

## 自定义修改

### 修改启动页
编辑 `app/src/main/res/values/styles.xml` 中的 `windowBackground`

### 修改状态栏颜色
编辑 `app/src/main/res/values/styles.xml` 中的 `statusBarColor`

### 修改应用图标
替换 `app/src/main/res/mipmap-*/ic_launcher.png` 和 `ic_launcher_round.png`
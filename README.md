# 和弦随机器 ChordRoller（Android App）

App 内置了和网页版完全相同的页面（`app/src/main/assets/index.html`）：
3 秒倒计时、节拍器"哒"声、滚轮调间隔、暂停/继续、练习记录、和弦类型范围选择。
练习时屏幕保持常亮。没联网也能用（只是字体换成系统字体）。

## 方式一：不装任何软件，用 GitHub 在线编译（推荐）
1. 注册/登录 github.com，点右上角 "+" → New repository，随便起个名字，建好。
2. 在仓库页面点 "uploading an existing file"，把解压后 `ChordRoller` 文件夹里的**所有内容**
   （包括 `.github` 文件夹）拖进去，点 Commit changes。
   注意：`.github` 是隐藏文件夹，Windows 需在资源管理器"查看"里勾选"隐藏的项目"才能看到。
3. 点仓库上方的 Actions，等 "Build APK" 出现绿色对勾（约 3–5 分钟）。
4. 点进这次运行，页面底部下载 `ChordRoller-apk`，解压得到 `app-debug.apk`。
5. 把 APK 发到手机安装（需允许"安装未知来源应用"）。

## 方式二：Android Studio
用 Android Studio 打开 `ChordRoller` 文件夹，连接手机点 ▶ Run，
或菜单 Build → Build APK(s)，APK 在 `app/build/outputs/apk/debug/`。

## 修改内容
直接改 `app/src/main/assets/index.html`，重新编译即可。

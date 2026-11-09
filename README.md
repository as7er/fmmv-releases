# FMMV · Football Manager Mobile Vibe

2D 足球经理生涯游戏：赛前布阵、临场战术、换人和实时比赛模拟。

本仓库仅用于**公开下载安装包、查看版本说明和反馈问题**。游戏源码仓库保持私有；此仓库不包含游戏源码或私有开发历史。公开安装包不代表游戏源码获得开源授权。

## Android 下载

- [查看全部版本](https://github.com/as7er/fmmv-releases/releases)
- [v0.3.0-android.2 防锁屏修复测试版](https://github.com/as7er/fmmv-releases/releases/tag/v0.3.0-android.2)
- [直接下载测试 APK](https://github.com/as7er/fmmv-releases/releases/download/v0.3.0-android.2/FMMV-0.3.0-android.2-debug.apk)

在 Release 页展开 **Assets**，下载以 `.apk` 结尾的文件。GitHub 自动生成的 `Source code.zip` / `tar.gz` 只包含本仓库的说明文件，不是游戏安装包，也不包含游戏源代码。

### 安装要求

- Android 7.0（API 24）或以上；Android System WebView 请保持更新。
- 下载后在手机文件管理器中打开 APK，按系统提示允许该来源安装应用。
- 不需要 Expo Go，也不需要电脑持续运行服务器；游戏资源随 APK 安装。
- 当前包使用 **Debug 测试签名**，属于 **Pre-release**，不是商店正式版。

## 测试版变化

- 手机比赛页实现自动横屏与沉浸式系统栏，退出比赛后恢复。
- Android构建号2修复观赛时自动熄屏：比赛页在前台保持亮屏，离开比赛或转后台后正常休眠，手动电源键锁屏不受影响。沿用原测试签名，直接覆盖安装，不要卸载旧版。
- 横屏采用左右操作栏，球场使用完整高度；保留完整球场比例，减少装饰看台。
- 844×390 视口下草皮面积较之前增加约 67%；常规桌面和平板保留原布局。

## 已知限制与存档提醒

- APK 构建、签名和包内资源检查已通过，生产网页手机交互已验证；**尚未完成 Android 真机／模拟器运行验证**。原生横屏、系统栏、返回和前后台恢复需实机验收。
- APK 与浏览器的存档独立，当前没有存档导入导出功能，不会自动迁移。
- 卸载应用或清除应用数据会删除本地存档；进行中的比赛不跨进程保存。
- 不要为安装测试包删除已有浏览器数据。若遇到签名不一致导致无法覆盖安装，不要先卸载，以免丢失存档。
- 客户端安装包中的代码可能被解包分析；不公开原始源码不等于客户端算法不可提取。

## 问题反馈

请在 [Issues](https://github.com/as7er/fmmv-releases/issues) 中提供手机型号、Android / WebView 版本、应用版本、复现步骤和截图。不要上传账号凭据、签名密钥或其他敏感信息。

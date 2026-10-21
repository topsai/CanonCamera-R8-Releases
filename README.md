# 佳能相机控制 · Android 安装包

这里仅公开APK、下载及更新说明，源码保存在私有仓库。

## 下载

当前开发预发布版本：**0.5.59**（2026-10-21）。

[下载0.5.59 APK](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.59) · [全部版本](https://github.com/topsai/CanonCamera-R8-Releases/releases) · [更新日志](#更新日志)

支持Android8.0及以上，设备需要USB Host/OTG。安装由Android系统确认；开发预发布版本并非所有设备都已完成实机验收。

## 更新日志

### 0.5.59 · 原生10×与视频斑马线

- 10×直接使用机身倍率指令，移除5×加App裁切；相机拒绝时保留原倍率。
- 视频设置新增斑马线，默认关闭，可选70/80/90/95/100%，保存选择；不改变机身录像或原片。
- 50项单元测试、5组模拟器UI回归通过；本轮未做机身10×及真机斑马线性能实测。

### 0.5.58 · 屏幕与大字体适配

- 小屏、矮横屏、大字体及平板窗口适配；修复录制时间边界和设置图标间距。
- 补回竖屏LUT效果选择入口，导入/管理仍在设置。
- 11组配置、126个监看组合及4组模拟器UI回归通过；本轮未做手机/相机实测。

### 0.5.57 · 启动自动检查更新

- 打开App后台检查新版本，不占用相机USB队列；有更新且前台空闲时提示，离线失败静默处理。
- 不自动下载或安装，保留设置中的手动检查。

### 0.5.56 · LUT设置入口

- LUT导入、管理和来源说明移入设置；保留已有文件和选择记录。

### 全部已公开版本

每个版本的完整变更、验证结果和未验证限制均放在对应Release正文，点下表进入；按版本号排序，避免把旧版本误作最新版本。

| 版本 | 发布日期（北京时间） | 更新说明 |
| --- | --- | --- |
| 0.5.59 | 2026-10-21 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.59) |
| 0.5.58 | 2026-10-21 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.58) |
| 0.5.57 | 2026-10-21 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.57) |
| 0.5.56 | 2026-10-19 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.56) |
| 0.5.55 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.55) |
| 0.5.54 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.54) |
| 0.5.53 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.53) |
| 0.5.51 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.51) |
| 0.5.50 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.50) |
| 0.5.49 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.49) |
| 0.5.48 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.48) |
| 0.5.47 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.47) |
| 0.5.46 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.46) |
| 0.5.45 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.45) |
| 0.5.44 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.44) |
| 0.5.43 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.43) |
| 0.5.42 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.42) |
| 0.5.41 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.41) |
| 0.5.40 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.40) |
| 0.5.39 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.39) |
| 0.5.38 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.38) |
| 0.5.37 | 2026-10-18 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.37) |
| 0.5.36 | 2026-10-17 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.36) |
| 0.5.35 | 2026-10-17 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.35) |
| 0.5.34 | 2026-10-17 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.34) |
| 0.5.33 | 2026-10-17 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.33) |
| 0.5.32 | 2026-10-17 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.32) |
| 0.5.31 | 2026-10-17 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.31) |
| 0.5.30 | 2026-10-17 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.30) |
| 0.5.29 | 2026-10-17 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.29) |
| 0.5.27 | 2026-10-17 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.27) |
| 0.5.26 | 2026-10-17 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.26) |
| 0.5.25 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.25) |
| 0.5.24 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.24) |
| 0.5.23 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.23) |
| 0.5.22 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.22) |
| 0.5.21 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.21) |
| 0.5.20 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.20) |
| 0.5.19 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.19) |
| 0.5.18 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.18) |
| 0.5.17 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.17) |
| 0.5.16 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.16) |
| 0.5.15 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.15) |
| 0.5.14 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.14) |
| 0.5.13 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.13) |
| 0.5.12 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.12) |
| 0.5.11 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.11) |
| 0.5.10 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.10) |
| 0.5.9 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.9) |
| 0.5.8 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.8) |
| 0.5.7 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.7) |
| 0.5.6 | 2026-10-16 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.6) |

## 应用内更新

从0.5.57起，打开App会在更新工作线程自动检查；有新版时在前台且拍摄/传输空闲后提示。也可在“设置 → 应用更新”或“参数 → 应用更新 / 检查新版”手动检查。无需GitHub登录。

下载后仍需系统安装确认，首次需允许此来源安装。普通应用不能静默安装；录像、拍摄或传输期间暂缓安装。旧版若没有更新入口，先从上方手动下载安装一次。

## 验证范围

以各版本Release说明为准。模拟器测试不等于真实手机、相机USB、对焦或取景性能已验证。这里只分发APK；GitHub自动生成的Source code包只包含本下载说明，不含App源码。

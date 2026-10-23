# 佳能相机控制 · Android 安装包

这里仅公开APK、下载及更新说明，源码保存在私有仓库。

## 下载

当前开发预发布版本：**0.5.65**（2026-10-23）。

[下载0.5.65 APK](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.65) · [全部版本](https://github.com/topsai/CanonCamera-R8-Releases/releases) · [更新日志](#更新日志)

支持Android8.0及以上，设备需要USB Host/OTG。安装由Android系统确认；开发预发布版本并非所有设备都已完成实机验收。

## 更新日志

### 0.5.65 · 修复R8一次性校时

- 修正R8未提供标准时间读取命令时无法校时的问题，使用已验证的Canon EOS路径。
- 手动点击仅同步一次，写入前核对时区，写入后重新请求回读；不会自动同步。
- 实体R8照片待机、+08:00时区下，App按钮校时后新请求回读与手机相差0秒；视频待机、其他机型/固件和时区仍待实测。
- 手机GPS仍未找到可验证的USB坐标写入接口，保持不可用；机身角度和原生时间码未接入。校时可能影响Free run时间码，请在非拍摄期间操作。

### 0.5.64 · 一次性相机校时

- 照片和视频设置加入“同步相机时间”按钮，每次点击仅同步一次，不自动校时。
- 拍摄、对焦、传输或已有待完成请求时不校时；成功提示需要相机回读确认。
- R8实际校时尚未实机验收。缺少可验证的时间读写或时区能力时会提示原因，不强行写入。
- 手机定位当前USB接口不可用，机身角度和原生时间码尚未接入；修改时间可能影响Free run时间码，请在非拍摄期间操作。

### 0.5.63 · 间隔拍摄与开关状态

- 将B门入口替换为间隔拍摄，可设置秒数与张数，运行中可停止。
- 由App计时，需要保持前台和USB连接；退到后台或断开会停止，相机忙/长曝光可能延长间隔。
- 自动对焦和自动传输开启时为绿色背景，关闭时为灰色。
- 此版间隔拍摄及开关显示仍待实体手机/相机复测。

### 0.5.62 · 统一设置布局

- 照片与视频设置统一为深色分组列表，统一字体、行高、图标和间距。
- 自动对焦、自动传输使用右侧开关；视频按LUT、视频监看、通用分组。
- 删除‘参数 / 诊断’入口；保留B门、LUT导入/管理、斑马线和应用更新。
- 横屏限宽并支持滚动；本次布局仍待实体手机复测。

### 0.5.61 · 按标记精简设置

- 删除圈内视频菜单入口，以及照片拍摄控制里的按钮和说明；保留“开始 B 门”、两个勾选项和应用更新。
- 视频设置保留应用更新、LUT导入/管理和视频斑马线。
- 此版B门、USB连接与录像尚未重新完成实机验收。

### 0.5.60 · 更新安装文件隔离

- 各版本使用独立校验文件和安装URI，修复固定地址复用旧安装内容的问题。
- 如果旧版提示安装相同版本，本次请直接下载0.5.60 APK覆盖安装，无需卸载或清除数据。
- 56项单元测试、6组模拟器回归及连续两次实际安装通过；原手机厂商安装器仍待复测。

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
| 0.5.65 | 2026-10-23 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.65) |
| 0.5.64 | 2026-10-23 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.64) |
| 0.5.63 | 2026-10-21 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.63) |
| 0.5.62 | 2026-10-21 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.62) |
| 0.5.61 | 2026-10-21 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.61) |
| 0.5.60 | 2026-10-21 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.60) |
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

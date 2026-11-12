# Android 更新日志

[返回主页](README.md) · [使用手册](docs/user-guide.md) · [全部版本](https://github.com/topsai/CanonCamera-R8-Releases/releases)

按版本从新到旧保留。各条目反映当时的功能与验证范围，不能当作所有旧功能仍然保留或本次重新验收。0.5.67已撤回公开下载。

## 0.5.85 · 2026-11-12

- 修复照片翻页时清空画面、出现整页读取提示的问题：下一张准备期间保留当前照片，方向处理好后再切换。
- 首次打开照片先保留相册并显示小型准备指示，预览就绪后进入大图，不再提前进入黑屏等待页。
- 视频支持左滑下一个、右滑上一个，按当前排序浏览视频；横屏点画面可显示或隐藏工具栏。
- 预览读取期间暂停下载、删除和保护操作，避免显示旧照片时误操作新文件。

## 0.5.84 · 2026-11-12

- 移除照片预览右上角齿轮，保留返回与底部信息、下载、删除。
- 照片信息栏新增照片自身的焦距；未提供时显示占位符。
- 照片预览支持左滑下一张、右滑上一张，跟随相册当前排序与筛选，跳过视频，首尾不循环。放大或双指操作时不翻页。
- 预览页照片下载固定保存为 JPG；相机只有 RAW 时提取其高清内嵌 JPEG，不改变相机原片。视频仍保存原文件。

- 横屏照片预览默认隐藏文件名栏和底部工具栏，单击图片切换；参数栏随之贴近图片边缘或避让按钮，返回按钮始终保留。
- 上一张、下一张增加平滑的淡入滑动动画；预览不再先显示方向不确定的缩略图，再突然转正。视频等待播放尺寸布局完成后开始播放。

## 0.5.83 · 2026-11-12

- 照片与视频预览底栏移除导出和重复的文件操作按钮，保留信息、下载、删除。
- 预览顶部及底部按钮栏改为半透明悬浮，减少占用画面空间；右上角文件操作入口保留。
- 照片信息仿照相机播放界面：上方显示序号和文件名，下方显示快门、光圈、曝光补偿、ISO及格式，横竖屏统一。
- 拍摄参数来自照片文件；未提供的数据以占位符显示，不使用相机当前设置代替。

## 0.5.82 · 2026-11-12

- 相册日期分组更紧凑，返回与底部工具栏统一为居中的纯图标按钮，修复预览页按钮大小不一致和重绘后消失。
- 点击照片先显示已有缩略图，支持的 CR3 直接读取内嵌高清 JPEG，减少等待；原片下载和导出保持独立。
- 视频增加缓冲、提前读取和按需缓存。根据文件时长及当前读取速度选择播放路径，高码率或缓冲不足时先缓存完整文件，以减少卡顿。
- 浏览相册时不再读取看不到的实时取景帧，返回拍摄页后恢复。
- 视频首播仍受手机解码能力、文件码率和 USB 速度影响，部分视频需要等待缓存。

## 0.5.80 · 2026-11-12

相机相册移除顶部信息和刷新栏，改用半透明悬浮返回箭头。在相册列表顶部向下拉再松手即可刷新，横屏可显示更多缩略图。

## 0.5.79 · 2026-11-12

竖屏拍摄页在相机型号后以小字显示当前 APK 版本号。 统一相机模式、显示模式和设置图标的视觉尺寸。

## 0.5.78 · 2026-11-12

照片和视频的档位文字加大并加粗，与设置齿轮形成更接近的视觉大小；横竖屏统一，较长档位名称自动适应按钮宽度。

## 0.5.77 · 2026-11-12

连接／断开按钮改为居中的 USB 三叉图标：未连接时为白色，已连接时显示绿色并带勾号，点击功能保持不变。照片模式图标扩大内部镂空，边框变薄并统一左右粗细。

## 0.5.76 · 2026-11-12

简化拍摄界面的按钮：档位仅显示 Av、M 等值；设置、相册和对焦移除文字，改用放大居中的图标。照片与视频横竖屏统一，按钮功能保持不变。照片／视频模式使用与机身拨杆相似的白色相机和摄像机图标。

本次图标调整尚未完成最终真机验收。

## 0.5.75 · 一体化显示模式图标

显示模式按钮改为一体化显示器图标：内部突出当前页数字、缩小总页数，取消图标下方重复文字。照片与视频横竖屏统一，点击切换和长按选择保持不变。

## 0.5.74 · 电池朝向与视频电量

- 调整相机电池图标朝向：右侧图标尖端朝左，照片参数页左下角图标保持朝右，均朝向屏幕内部。
- 视频显示2新增电量图标，位于右下角焦距上方；显示3新增电量图标，位于参数页右下角，横竖屏一致。保留70%尺寸、电量格数和绿黄红颜色，显示1保持不变。

## 0.5.73 · 照片简洁显示与电池图标

- 照片新增第 4 种「简洁参数」显示模式：隐藏取景左右两列参数，保留档位、剩余张数、电池、焦距、快门、光圈、曝光尺、ISO 和对焦框，横竖屏一致。点击显示按钮切换，长按可直接选择。视频仍保留原有三种模式。
- App 内相机电池图标等比例缩小 30%，保留电池格数与绿、黄、红颜色提示。

## 0.5.72 · 自动 ISO 显示时机

修复照片自动 ISO 数值被 App 的 2 秒超时提前清除的问题。收到有效测光值后持续显示；机身结束测光并回报 AUTO 时恢复自动显示，与机身状态同步。

## 0.5.71 · 自动 ISO 读数

照片模式使用自动 ISO 时，收到有效测光读数便显示具体数值，例如 `AUTO 1600`。读数缺失、失效或过期时恢复原来的自动 ISO 显示。R8 实机回传待复测。

## 0.5.70 · 照片 EXIF、拍后回看与自动 ISO

- 仅 RAW 时导出内嵌 JPG，会保留源文件提供的机身、镜头、拍摄时间、焦距、光圈、快门、ISO 和方向。机身 JPG 直接保存。
- 照片设置新增「拍后回看」，默认 2 秒，可选关闭或 1–5 秒。机身提供缩略图时会在取景区显示刚拍的照片。
- 照片模式使用自动 ISO 时，机身同时提供合焦状态和有效测光 ISO 即显示具体数值。

已用真实 CR3 文件离线核对导出 JPG 的 EXIF。手机相册界面、回看及 R8 实时 ISO 触发时机待实机验证。

## 0.5.69 · 电池格数与电量颜色

- 将电量百分比改为电池格数，避免把机身分档误认为精确电量。
- 3–4 格绿色、2 格黄色、1 格及低电量红色；无有效读数或断开时为灰色未知状态。
- 保留原有电池图标的位置与大小，更新图文手册中的电量说明。

已在 Android 15 手机上检查各档位的实际绘图。本次未进行相机完整放电测试；格数依赖机身提供的电量档位，不代表线性续航或精确百分比。

## 0.5.68 · 修正10×实际显示区域

- 按机身指定的有效区域显示R8的10×取景，修复其画面与5×相同的问题。
- 保留原生倍率指令、机身倍率回读，以及暂停取景/切后台后恢复1×的修复。
- 保留完整原片缓存身份校验和不同USB会话隔离。

已在R8与Android 15手机上，通过App按钮验证照片/视频、横屏/竖屏的1×、5×、10×。其他机型或不同取景数据布局尚未确认。

## 0.5.67 · 已撤回公开下载

发现5×与10×实际画面区分异常，暂停公开下载及应用内更新提示，待修复后发布新的版本号。

- 修复相机相册预览、下载可能误用其他照片缓存的问题；缓存增加完整身份核对与USB会话隔离。
- 修复照片和视频模式在5×、10×暂停取景或切后台后，App显示1×而机身仍保留放大的问题。
- 恢复取景前刷新机身输出状态；倍率切换期间等待对应画面确认，避免旧放大帧被当作完整画面用于点击对焦。
- 重连后首次打开原片会重新从相机读取，同一连接内仍可复用已确认缓存。

已在实体R8的照片/视频待机下验证5×、10×恢复及后台返回。未验证录像中后台切换及其他机型/固件的相同行为。

## 0.5.66 · 精简相机同步设置

- 删除照片和视频设置中校时下方的固定说明、手机定位开关及定位不可用说明。
- 保留同步时间按钮和动态结果，不自动校时；本次不改变校时协议。
- GPS仍未实现，未新增定位权限或后台定位。校时可能影响Free run时间码，请在非拍摄期间操作。

## 0.5.65 · 修复R8一次性校时

- 修正R8未提供标准时间读取命令时无法校时的问题，使用已验证的Canon EOS路径。
- 手动点击仅同步一次，写入前核对时区，写入后重新请求回读；不会自动同步。
- 实体R8照片待机、+08:00时区下，App按钮校时后新请求回读与手机相差0秒；视频待机、其他机型/固件和时区仍待实测。
- 手机GPS仍未找到可验证的USB坐标写入接口，保持不可用；机身角度和原生时间码未接入。校时可能影响Free run时间码，请在非拍摄期间操作。

## 0.5.64 · 一次性相机校时

- 照片和视频设置加入“同步相机时间”按钮，每次点击仅同步一次，不自动校时。
- 拍摄、对焦、传输或已有待完成请求时不校时；成功提示需要相机回读确认。
- R8实际校时尚未实机验收。缺少可验证的时间读写或时区能力时会提示原因，不强行写入。
- 手机定位当前USB接口不可用，机身角度和原生时间码尚未接入；修改时间可能影响Free run时间码，请在非拍摄期间操作。

## 0.5.63 · 间隔拍摄与开关状态

- 将B门入口替换为间隔拍摄，可设置秒数与张数，运行中可停止。
- 由App计时，需要保持前台和USB连接；退到后台或断开会停止，相机忙/长曝光可能延长间隔。
- 自动对焦和自动传输开启时为绿色背景，关闭时为灰色。
- 此版间隔拍摄及开关显示仍待实体手机/相机复测。

## 0.5.62 · 统一设置布局

- 照片与视频设置统一为深色分组列表，统一字体、行高、图标和间距。
- 自动对焦、自动传输使用右侧开关；视频按LUT、视频监看、通用分组。
- 删除‘参数 / 诊断’入口；保留B门、LUT导入/管理、斑马线和应用更新。
- 横屏限宽并支持滚动；本次布局仍待实体手机复测。

## 0.5.61 · 按标记精简设置

- 删除圈内视频菜单入口，以及照片拍摄控制里的按钮和说明；保留“开始 B 门”、两个勾选项和应用更新。
- 视频设置保留应用更新、LUT导入/管理和视频斑马线。
- 此版B门、USB连接与录像尚未重新完成实机验收。

## 0.5.60 · 更新安装文件隔离

- 各版本使用独立校验文件和安装URI，修复固定地址复用旧安装内容的问题。
- 如果旧版提示安装相同版本，本次请直接下载0.5.60 APK覆盖安装，无需卸载或清除数据。
- 56项单元测试、6组模拟器回归及连续两次实际安装通过；原手机厂商安装器仍待复测。

## 0.5.59 · 原生10×与视频斑马线

- 10×直接使用机身倍率指令，移除5×加App裁切；相机拒绝时保留原倍率。
- 视频设置新增斑马线，默认关闭，可选70/80/90/95/100%，保存选择；不改变机身录像或原片。
- 50项单元测试、5组模拟器UI回归通过；本轮未做机身10×及真机斑马线性能实测。

## 0.5.58 · 屏幕与大字体适配

- 小屏、矮横屏、大字体及平板窗口适配；修复录制时间边界和设置图标间距。
- 补回竖屏LUT效果选择入口，导入/管理仍在设置。
- 11组配置、126个监看组合及4组模拟器UI回归通过；本轮未做手机/相机实测。

## 0.5.57 · 启动自动检查更新

- 打开App后台检查新版本，不占用相机USB队列；有更新且前台空闲时提示，离线失败静默处理。
- 不自动下载或安装，保留设置中的手动检查。

## 0.5.56 · LUT设置入口

- LUT导入、管理和来源说明移入设置；保留已有文件和选择记录。

### 全部已公开版本

每个版本的完整变更、验证结果和未验证限制均放在对应Release正文，点下表进入；按版本号排序，避免把旧版本误作最新版本。

| 版本 | 发布日期（北京时间） | 更新说明 |
| --- | --- | --- |
| 0.5.66 | 2026-10-23 | [查看更新日志](https://github.com/topsai/CanonCamera-R8-Releases/releases/tag/android-v0.5.66) |
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

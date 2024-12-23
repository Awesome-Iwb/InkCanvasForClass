# FAQ

## 1. ICC 对 PPT 的相容性如何呢？

ICC 可以支持 WPS，但目前无法同时支持 MSOffice 和 WPS。若要启用 WPS 支持，请确保 WPS 是否在 “配置工具” 中开启了 “WPS Office 相容第三方系统和软件” 选项，该项目勾选并应用后，将无法检测到 MS Office 的COM接口。

如果您安装了“赣教通”、“畅言智慧课堂”等应用，可能会安装“畅言备课精灵”，因此会导致遗失64位的 Office COM 组件的注册且目前似乎无法修复（可以切换到新用户正常使用）。但 WPS Office 可以正常使用。

若要将 ICC 配合 WPS 使用，可打开“WPS 演示”后，前往“文件” - “选项” ，取消勾选“单萤幕幻灯片放映时，显示放映工具栏”该项，获得更好的体验。若要将 ICC 配合 MS Office 使用，可以打开 Powerpoint，前往“选项” ，“高级”，取消勾选“显示快捷工具栏”，获得更好的体验。

> 不建议使用 WPS，因为 WPS 会污染系统的 COM 接口环境，而且 WPS 简直就是像素级抄袭 Office，用了会让你痛恨一辈子。

## 2. **安装后**程序无法正常启动？

请检查你的电脑上是否安装了 `.Net Framework 4.7.2` 或更高版本。若没有，请前往官网下载。

如果程序在启动后黑屏闪退，请打开 “事件查看器” 搜索有关 InkCanvasForClass 的错误信息并上报给开发者（可以在 GitHub 上提交 Issue，或者和开发者单独沟通）

Windows 7 和 8/8.1 系统可能会出现无法启动的问题，属于正常情况（因为开发者还没有对旧版本系统进行优化，会因为部分依赖 Windows 10+ 系统的 API 导致 ICC 无法启动！

> 遇到各种奇葩逗比问题请重启应用程式，如果不行请反馈给Dev解决！

## 3. ICC 什么时候发正式版

取决于什么时候 ICC 能够达到我心中期待的样子

## 4. 我为什么要用 ICC ？

ICC 的开发意图，是为了把 IC 和 ICA 的优点融合起来，修复他们的缺点，并在 ICA 的代码基础上进行改善和重写（其实现在很多 ICC 的代码都已经被逗比重写了，已经逐渐和 ICA 脱离干系了），使其功能更加丰富强大，接近于一个商业产品的完善度，如果你觉得 ICC 不适合你，那欢迎你使用同类产品。

## 5. ICC 目前只能用 Visual Studio 编译使用吗？

对，我主观意识上并不想提供非正式版的 build，即使前面一段时间有机器人自动构建（虽然自动构建使用的是能工智人，~~`而且还是司马的幻想熵`~~，但毕竟不是我自己来构建的），但我并不想让大家使用一个还在开发的不完整的有缺陷的软件。具体请参考 Salt Player for Windows 的开发者阐述的观点，我和他的比较类似。

## 6. 用管理员权限运行 ICC 后，PPT 批注功能失效了

已知问题，目前正在重写 PPT 模块实现自动降权来解决。

## 附：ICC 画的所有饼

- 浮动工具栏 UI 改进（正在填屎坑）
- 白板模式 UI 改进（还有背景色和稿纸模式）
- **鼠标手势**，可以让画布移动缩放，甚至是旋转，都变得更加轻松（正在开发）
- **全新的设置 UI**，正在逐步清理原项目的屎山
- **强制置顶**，基于 UIAccess + 输入线程抢夺的方法，保证 ICC 永远显示在所有软件的最顶层
- **分辨率和DPI变化监听**，保证 ICC 界面正常显示
- **高性能透明**，绘制使用多线程 UI + WindowChrome，摆脱低性能体验
- **画面冻结**，使当前画面定格
- **重写形状绘制**，让绘图体验更舒适方便，还会支持函数绘制和物理图绘制
- **PPT COM+VSTO双接口融合**，缓解 Office 和 WPS 共存导致的 COM 接口被占用的问题
- **PPT 系统优化**，高效 PPT 放映状态检测，不丢页不跳页
- **禁用边缘手势**，禁用烦人的 Windows10/11 的边缘触摸手势
- **点名器优化**，将会支持历史记录和多名单抽选，同时支持特殊配置
- **内置小工具**，内置计算器，英汉词典，倒计时，秒表，放大镜，截图等实用小工具
- **QuickPanel**，方便快捷的从 ICC 打开所有应用和调整系统设置
- **情境化配置**，每位老师都有专属的配置文件
- **插件和脚本系统**，支持使用 dotNet Framework 开发原生扩展或使用 Javascript 开发脚本来实现自动化操作或其他扩充功能
- **形状识别**，基于微软清朝老库的手绘形状自动识别，并提供形状绘制纠正功能
- **板书库**，高效管理所有板书，课程自动分类，提供云端同步
- **自动收纳**，检测到教学软件自动开启时会自动隐藏 ICC 界面到屏幕侧边
- **自动查杀**，检测到指定软件可以让 ICC 大打出手直接查杀并自动使用 ICC 进行替代
- **桌面悬浮窗屏蔽**，隐藏画板悬浮窗，还您一个干净的电脑桌面
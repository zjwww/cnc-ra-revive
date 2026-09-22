<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/logo-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="assets/logo-light.svg">
    <img src="assets/logo-light.svg" width="96" alt="CnC-RA-Revive CR command logo">
  </picture>
  <h1>CnC-RA-Revive</h1>
  <p>展示《命令与征服》／《红色警戒》与 OpenTS、OpenRA、Chrono Divide 之间关系的信息图。</p>
  <p>
    <img src="https://img.shields.io/badge/version_EN-1.12--en-00a85a?style=flat" alt="English version 1.12-en">
    <img src="https://img.shields.io/badge/version_ZH-1.11-00a85a?style=flat" alt="Chinese version 1.11">
    <img src="https://img.shields.io/badge/platform-desktop_%7C_mobile-276bd1?style=flat" alt="Platform: desktop and mobile browsers">
    <img src="https://img.shields.io/badge/runtime-browser_JavaScript-f0db4f?style=flat" alt="Runtime: browser JavaScript">
    <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT_(project--owned)-blue?style=flat" alt="License: MIT for project-owned contributions; see scope"></a>
  </p>
  <p><a href="README.md">English</a> | <a href="README.zh-CN.md">简体中文</a> | <a href="https://zjwww.github.io/cnc-ra-revive/">已发布网站</a> | <a href="https://github.com/zjwww/cnc-ra-revive/issues">问题反馈</a></p>
</div>

[![中文信息图缩略图](preview.webp)](https://zjwww.github.io/cnc-ra-revive/index.html)

960 × 540 WebP 仅用于文档预览。[更新日志](CHANGELOG.zh-CN.md)。

**已发布版本：英文 v1.12-en · 简体中文 v1.11。** 网站首页继续使用完全未变的中文 v1.11 原生缩放页。每种语言均提供两套缩放机制、四个独立 HTML/SVG 文件，保留 3840 × 2160 坐标系、16:9 比例、177 个文字位置和固定布局。英文版翻译文字并调整部分字号，查看器脚本和图像几何位置不变。

英文 v1.12-en 已完成 150% 显示缩放下的 32 项桌面检查、四个文件默认截图一致性检查、44 处链接检查／48 次新标签页打开，以及四个英文文件的移动端模拟检查。这些是已有本地验证记录，本次没有新增 iPhone／Safari 真机测试。

## 浏览器标签页标题

两个格式统一采用 `CnC-RA-Revive · Native Scale` 或 `CnC-RA-Revive · Viewer Scale`。桌面的 Viewer Scale 组在标题后附加页面内倍率，例如 `CnC-RA-Revive · Viewer Scale 110%`；Native Scale 不重复显示浏览器菜单倍率。手机标题保留模式名，不显示百分比。信息图正文保持不变。

## 选择版本

| 语言／版本 | 缩放机制 | HTML | SVG |
| --- | --- | --- | --- |
| 简体中文 v1.11 | 浏览器原生缩放 | [HTML](https://zjwww.github.io/cnc-ra-revive/index.html) | [SVG](https://zjwww.github.io/cnc-ra-revive/CnC-RA-Revive-4k-Native.svg) |
| 简体中文 v1.11 | 页面内代码缩放 | [HTML](https://zjwww.github.io/cnc-ra-revive/CnC-RA-Revive-4k-Viewer.html) | [SVG](https://zjwww.github.io/cnc-ra-revive/CnC-RA-Revive-4k-Viewer.svg) |
| 英文 v1.12-en | 浏览器原生缩放 | [HTML](https://zjwww.github.io/cnc-ra-revive/CnC-RA-Revive-4k-Native-EN.html) | [SVG](https://zjwww.github.io/cnc-ra-revive/CnC-RA-Revive-4k-Native-EN.svg) |
| 英文 v1.12-en | 页面内代码缩放 | [HTML](https://zjwww.github.io/cnc-ra-revive/CnC-RA-Revive-4k-Viewer-EN.html) | [SVG](https://zjwww.github.io/cnc-ra-revive/CnC-RA-Revive-4k-Viewer-EN.svg) |

SVG 请直接在浏览器标签页中打开，以使用交互功能。每个 HTML、SVG 均内嵌图片和脚本，可单独使用，不依赖相邻文件或网络连接。同一套中的两个格式使用完全相同的查看器代码。

## 非整数显示缩放

桌面宽度适配改用带小数精度的可用视口宽度，避免 `clientWidth` 整数取整误差；图像宽度向下对齐到物理像素，高度按相同的 16:9 比例计算。修复了适配尺寸下不足一个像素的溢出引起横向滚动条的问题，覆盖 4K 窗口及 150% 显示缩放等情况。边缘最多保留不足一个物理像素的余量；浏览器不支持 Visual Viewport API 时，保守预留一个 CSS 像素。

没有隐藏横向溢出：主动进行原生或页面内放大后，仍可横向滚动到右边缘。手机端稳定视口测量和浏览器原生手势保持不变，v1.9 的 11 处链接及提示取消改动全部保留。

## 项目超链接

八个 HTML/SVG 文件均保留 11 处项目文字链接。鼠标悬停时显示下划线及目标地址提示，键盘聚焦时也显示下划线。点击通过 `target="_blank"` 请求在新标签页打开，原信息图保留；实际使用新标签页还是新窗口由浏览器偏好设置决定。

右侧三个标题分别链接至 OpenTS GitHub 仓库、OpenRA 官网和 Chrono Divide 官网；底部表头分别链接至 OpenTS GitHub 仓库、OpenRA GitHub 仓库和 Chrono Divide GitHub 组织。EA 四个源码名称及 `CnC_Modding_Support` 分别链接到 Electronic Arts 对应的 GitHub 仓库。

HTML 使用 head 中的文档标题，独立 SVG 使用根元素中的文档标题；HTML 内嵌 SVG 不设置根标题，以避免整图悬停提示。项目链接保留目标地址提示。SVG 请直接作为文档打开，以使用链接和查看器交互。

## iPhone／触屏浏览

八个文件均将手机双指缩放和平移交给浏览器。页面内缩放组仅在桌面继续使用代码处理滚轮与快捷键。手机标签页采用同样的英文模式名，不显示百分比；两组的触屏手势仍由浏览器原生处理。

首次适配优先采用稳定的小视口 CSS 宽度（`svw`）；稳定高度（`svh`）也用于旋转后的稳定性检查。双指缩放、拖动和工具栏引起的单纯高度变化不重写图像尺寸。屏幕旋转或真实布局宽度变化后，等待约 150 毫秒稳定，再连续核对两帧；1 个 CSS 像素以内的差异视为误差。一次检查超过 800 毫秒仍未稳定就放弃，不会在手势期间强制适配；后续有效事件可重新发起检查。

手机端不取消触摸或手势默认行为，不重置浏览器倍率，也不调用 `scrollTo()`。旋转后图中某个点能否留在原位置由 Safari 的缩放和滚动恢复决定，不能保证精确保留；新方向稳定后，适配尺寸可能调整一次。不支持小视口单位时，保守地仅在首次打开和方向变化时适配。

v1.7 移动端候选版已由用户在反馈的 iPhone 14 Pro／iOS 26.6.2 上试用，未发现新的问题。当前版本保留该手势处理及按宽度适配；本次桌面及移动端自动化模拟不能替代新适配方式的真机测试。原图、箭头修复和 16:9 坐标保持不变。

## 桌面缩放行为

| 操作 | 原生缩放组 | 页面内缩放组 |
| --- | --- | --- |
| Ctrl + 滚轮、Ctrl + 加减键 | 浏览器处理缩放，菜单百分比随之变化。 | 代码按 25%～500% 缩放图像，浏览器百分比保持原值。 |
| Ctrl + 0 | 浏览器恢复 100%。 | 图像恢复按宽度适配，并滚动回左上角。 |
| 倍率显示 | 浏览器缩放菜单。 | HTML 与 SVG 标签页标题，例如“CnC-RA-Revive · Viewer Scale 150%”。 |
| 调整窗口大小 | 适配基准随窗口调整，保留相对原生缩放。 | 重新计算适配尺寸，保留所选页面内倍率。 |
| 刷新 | 会话存储可用时，保留原生缩放的适配基准。 | 页面内倍率恢复为适配窗口的初始值。 |

八个文件初始均**按可用视口宽度适配**，图像高度为宽度的 9/16；窗口高度不足时纵向滚动查看。图像不会拉伸、裁切或重排模块。桌面缩放以按宽度适配的尺寸为基准，放大后可用普通滚动查看其余部分；手机双指缩放仍交给浏览器。

### 原生版适配基准

原生组不拦截滚轮与快捷键的默认行为。少量脚本只负责等比尺寸计算，不设置或模拟浏览器菜单百分比。标签页首次访问时，按浏览器**当前**缩放与显示缩放建立适配基准；支持会话存储时，刷新会保留该基准。

为便于四个文件对比，建议先将浏览器设为 **100%，再用新标签页打开文件**。首次在 150% 的新标签页打开，会以初始 150% 为适配基准；这与先在 100% 打开、再放大至 150% 的显示尺寸不同。Ctrl + 0 始终重置浏览器倍率，不重新定义已保存的适配基准。禁用会话存储时，刷新会重新建立基准。跨不同显示缩放的显示器移动窗口尚未验证，可在目标显示器使用新标签页重新建立基准。

### 页面内操作与兼容性

使用快捷键前先让文档获得焦点。支持 Ctrl + 等号和数字小键盘加减键。滚轮缩放尽量保持鼠标指向的图内位置，受滚动边界限制；键盘缩放以可视区域中心为锚点。HTML 与独立 SVG 标签页均显示桌面页面内倍率，不代表浏览器倍率。直接操作浏览器菜单仍属于另一套浏览器操作。

共同的尺寸适配及页面内交互需要 JavaScript。SVG 作为独立交互文档打开时可运行脚本；通过 HTML 图片元素嵌入时脚本会被禁用，成为静态图像。八个文件中的图像仍保留可编辑的 SVG 文字与素材。

## 信息图内容

- 《命令与征服》、泰伯利亚之日和火线风暴。
- 《红色警戒》《红色警戒 2》和尤里的复仇。
- EA 已公开源码仓库，以及完整引擎源码与 Mod 资源的区别。
- OpenTS 的源码重建、OpenRA 的现代化再演绎、Chrono Divide 的浏览器 RA2 路线。
- 彩色关系箭头、源码状态标签和项目对比表。

本仓库发布的是说明性信息图，不包含可玩的游戏、游戏引擎实现或原版游戏数据。

## 文件与版本保留

中文 v1.11 包含 `index.html`、`CnC-RA-Revive-4k-Native.svg`、`CnC-RA-Revive-4k-Viewer.html` 和 `CnC-RA-Revive-4k-Viewer.svg`。英文 v1.12-en 新增 `CnC-RA-Revive-4k-Native-EN.html`、`CnC-RA-Revive-4k-Native-EN.svg`、`CnC-RA-Revive-4k-Viewer-EN.html` 和 `CnC-RA-Revive-4k-Viewer-EN.svg`。仓库包含各语言对应的 WebP 缩略图、浅深色 SVG Logo 和双语文档。完整 PNG 导出、Logo 方案板、工作脚本和历代版本目录仅在本地保留；以前发布过的文件仍可通过 Git 历史查看。

## 后期编辑

重要文字、表格内容、边框和箭头均为可编辑 SVG 元素。可使用 UTF-8 文本编辑器或支持 SVG 的编辑器，修改 SVG 副本或 HTML 内嵌的 SVG。HTML 目前是静态查看页面，不支持直接点击文字编辑或在浏览器内保存修改。

请保留 `0 0 3840 2160` 的 viewBox、等比缩放设置和查看器操作逻辑。修改文字后，检查换行、边界和图片区是否被遮挡。HTML 与 SVG 是独立文件，新版本需要有意识地同步修改两份内容。导出 PNG 时应明确指定 **3840 × 2160**；其他窗口尺寸下的浏览器截图会采用对应窗口尺寸。

## 内容范围与视觉限制

内容是 2026 年 9 月整理的说明性快照，不是实时状态监控，也不是完整的技术审计。“原始源码已丢失”等较强结论沿用了原始信息图需求，本仓库没有独立证明这些历史判断。没有公开发布源码，本身不等于所有原始源码副本均已丢失。保真度属于定性评价，兼容情况也可能变化。

背景、游戏风格插画和徽标包含 AI 重绘内容，可能与官方美术有所不同。文字和图表几何元素在 3840 × 2160 画布上重新渲染，但装饰位图素材为 1672 × 941，**并非全部素材都原生达到 4K**。整张信息图经过重新构建，并非对参考原图简单放大。字体使用系统字体，主要为微软雅黑和 Arial；缺少相应字体的系统可能呈现不同效果。

由于内嵌图片，独立 HTML 和 SVG 文件各约 10 MB。

## 上游参考

当前项目状态和技术细节请以上游说明为准：

- [EA：CnC_Tiberian_Dawn](https://github.com/electronicarts/CnC_Tiberian_Dawn)：官方公开源码仓库。
- [OpenTS](https://github.com/OpenTS-Developers/OpenTS)：泰伯利亚之日重建项目及文档。
- [OpenRA 项目介绍](https://www.openra.net/about/)：项目目标与现代化玩法。
- [Chrono Divide](https://chronodivide.com/)：浏览器中的《红色警戒 2》项目。
- [Chrono Divide Mod SDK](https://github.com/chronodivide/mod-sdk)：Mod 兼容情况与限制。

## 网站托管

GitHub Pages 从 `main` 分支根目录发布。默认首页仍为中文 v1.11 原生 HTML，本次英文发布不修改该页面。英文 v1.12-en 通过上方版本表进入，查看器内不添加语言开关。

## 署名与许可

这是独立的社区信息图项目，与 Electronic Arts、OpenTS、OpenRA 和 Chrono Divide 没有隶属关系，也不代表这些项目的背书。游戏名称、商标、项目名称及第三方视觉标识的权利归其各自权利人所有。

项目自有的查看器代码、文档、原创图表文字／几何元素及原创 Logo 贡献采用 [MIT 许可证](LICENSE)，仅限贡献者实际拥有且可授予的权利；具体排除范围见[许可范围说明](LICENSING.zh-CN.md)。第三方游戏美术、名称、商标、Logo 和上游素材不由本项目授权。AI 辅助生成的图像不保证具有排他版权或已获得第三方许可，收录不代表授予贡献者并不拥有的权利。上游项目继续适用各自许可证。

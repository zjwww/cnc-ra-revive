# cnc-ra-revive

[在线查看](https://zjwww.github.io/cnc-ra-revive/) · [更新日志](CHANGELOG.zh-CN.md) · [English](README.md)

一张展示 EA **《命令与征服》／《红色警戒》**与 **OpenTS、OpenRA、Chrono Divide** 之间关系的信息图。以科幻 RTS 风格呈现官方游戏系列、源码状态标签、社区开发路线和项目对比。

**当前版本：v1.2。** 信息图采用简体中文，并保留英文游戏名和项目名。英文 README 介绍的是同一份作品，并不代表图中内容已有英文翻译版。

## 查看与缩放

- [打开 HTML 在线网页](https://zjwww.github.io/cnc-ra-revive/)。
- [打开最新版独立 SVG](https://zjwww.github.io/cnc-ra-revive/RA-4K.svg)。

HTML 打开时自动适配窗口宽度。必要时先点击页面内部，再使用以下操作：

| 操作 | 效果 |
| --- | --- |
| `Ctrl` + 鼠标滚轮 | 围绕鼠标指针放大或缩小整张信息图。 |
| `Ctrl` + `+` / `-` | 放大／缩小；同时支持 `Ctrl` + `=` 和数字小键盘加减键。 |
| `Ctrl` + `0` | 恢复适配窗口，并回到左上角。 |
| 普通滚轮／滚动条 | 在放大后的信息图中移动查看。 |

缩放范围为适配尺寸的 25%～500%，始终保持 **16:9** 比例及所有模块的位置。调整窗口大小会保留当前相对缩放倍数；刷新页面恢复适配窗口。

HTML 快捷键控制的是**页面内整图缩放**，不会修改浏览器缩放菜单显示的百分比。操作时焦点应在网页内部，而不是地址栏或浏览器菜单。SVG 继续使用浏览器原生缩放。HTML 的整图缩放需要 JavaScript；禁用 JavaScript 后，仍可查看自动适配窗口的信息图。

两个文件均内嵌所需素材，也可在本地直接打开。不需要安装、构建、框架、账号或额外下载图片。

## 预览

这张 960 × 540 的 WebP 缩略图约 106 KiB，点击可进入完整网页。当前仓库文件列表不包含完整尺寸的 PNG 导出图。

[![命令与征服及红色警戒社区项目关系图](preview.webp)](https://zjwww.github.io/cnc-ra-revive/)

## 信息图内容

- 《命令与征服》、泰伯利亚之日和火线风暴。
- 《红色警戒》《红色警戒 2》和尤里的复仇。
- EA 已公开源码仓库，以及完整引擎源码与 Mod 资源的区别。
- OpenTS 的源码重建、OpenRA 的现代化再演绎、Chrono Divide 的浏览器 RA2 路线。
- 彩色关系箭头、源码状态标签和项目对比表。

本仓库发布的是说明性信息图，不包含可玩的游戏、游戏引擎实现或原版游戏数据。

## 文件与版本保留

| 路径 | 用途 |
| --- | --- |
| `index.html` | 最新版自适应 HTML，支持整图缩放操作。 |
| `RA-4K.svg` | 最新版自适应、可编辑的独立 SVG。 |
| `preview.webp` | README 使用的小尺寸缩略图。 |
| `README.md` / `README.zh-CN.md` | 英文和简体中文项目说明。 |
| `CHANGELOG.md` / `CHANGELOG.zh-CN.md` | 对应的双语版本记录。 |
| `.nojekyll` | 用于 GitHub Pages 直接发布静态文件。 |

GitHub 当前文件列表仅保留最新 HTML、SVG、小尺寸预览图、文档和仓库配置，不再包含 `v1.0`／`v1.1` 目录及完整 PNG 导出图。历史文件仍可从旧 Git 提交查看，没有重写 Git 历史。

本地工作副本继续按照 **v1.0、v1.1、v1.2、v1.3 等目录**分别保留各版文件。后续更新保留本地归档，替换 GitHub 根目录的当前版本文件，并同步更新两份日志。这个静态网站暂不使用 GitHub Release。

## 后期编辑

重要文字、表格内容、边框和箭头均为可编辑 SVG 元素。可使用 UTF-8 文本编辑器或支持 SVG 的编辑器，修改 SVG 副本或 HTML 内嵌的 SVG。HTML 目前是静态查看页面，不支持直接点击文字编辑或在浏览器内保存修改。

请保留 `0 0 3840 2160` 的 viewBox、等比缩放设置和查看器操作逻辑。修改文字后，检查换行、边界和图片区是否被遮挡。HTML 与 SVG 是独立文件，新版本需要有意识地同步修改两份内容。导出 PNG 时应明确指定 **3840 × 2160**；其他窗口尺寸下的浏览器截图会采用对应窗口尺寸。

## 内容范围与视觉限制

内容是 2026 年 9 月整理的说明性快照，不是实时状态监控，也不是完整的技术审计。“原始源码已丢失”等较强结论沿用了原始信息图需求，本仓库没有独立证明这些历史判断。没有公开发布源码，本身不等于所有原始源码副本均已丢失。保真度属于定性评价，兼容情况也可能变化。

背景、游戏风格插画和徽标包含 AI 重绘内容，可能与官方美术有所不同。文字和图表几何元素在 3840 × 2160 画布上重新渲染，但装饰位图素材为 1672 × 941，**并非全部素材都原生达到 4K**。整张信息图经过重新构建，并非对参考原图简单放大。字体使用系统字体，主要为微软雅黑和 Arial；缺少相应字体的系统可能呈现不同效果。

由于内嵌图片，独立 HTML 和 SVG 文件各约 10 MB。后续版本可考虑共用并优化图片资源，以改善加载速度，同时保留已有归档。

## 上游参考

当前项目状态和技术细节请以上游说明为准：

- [EA：CnC_Tiberian_Dawn](https://github.com/electronicarts/CnC_Tiberian_Dawn)：官方公开源码仓库。
- [OpenTS](https://github.com/OpenTS-Developers/OpenTS)：泰伯利亚之日重建项目及文档。
- [OpenRA 项目介绍](https://www.openra.net/about/)：项目目标与现代化玩法。
- [Chrono Divide](https://chronodivide.com/)：浏览器中的《红色警戒 2》项目。
- [Chrono Divide Mod SDK](https://github.com/chronodivide/mod-sdk)：Mod 兼容情况与限制。

## 网站托管

GitHub Pages 使用 `main` 分支的仓库根目录作为发布来源。网站通过 `index.html` 展示信息图；GitHub 仓库首页仍默认展示 `README.md`。`.nojekyll` 用于禁用 Jekyll 处理。相关配置见 [GitHub Pages 官方说明](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)。

## 署名与许可

这是独立的社区信息图项目，与 Electronic Arts、OpenTS、OpenRA 和 Chrono Divide 没有隶属关系，也不代表这些项目的背书。游戏名称、商标、项目名称及第三方视觉标识的权利归其各自权利人所有。

本仓库暂未选定统一的再分发许可。公开可访问不应被理解为对第三方美术或标识的统一授权。各上游项目有其各自的许可证，这些许可证不会自动适用于本信息图。

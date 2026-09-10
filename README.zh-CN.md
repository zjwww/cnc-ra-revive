# cnc-ra-revive

[在线查看](https://zjwww.github.io/cnc-ra-revive/) · [更新日志](CHANGELOG.zh-CN.md) · [English](README.md)

一张展示 EA **《命令与征服》／《红色警戒》**与 **OpenTS、OpenRA、Chrono Divide** 之间关系的信息图。以科幻 RTS 风格呈现官方游戏系列、源码状态标签、社区开发路线和项目对比。

**当前版本：v1.1。** 信息图采用简体中文，并保留英文游戏名和项目名。英文 README 介绍的是同一份作品，并不代表图中内容已有英文翻译版。

## 查看方式

- [打开在线网页](https://zjwww.github.io/cnc-ra-revive/)。
- [打开 v1.1 HTML 固定版本地址](https://zjwww.github.io/cnc-ra-revive/v1.1/RA-4K.html)。
- [打开 v1.1 自适应 SVG](https://zjwww.github.io/cnc-ra-revive/v1.1/RA-4K.svg)。
- [查看最初的 3840 × 2160 PNG](v1.0/RA-4K.png)。

HTML 和独立 SVG 都会根据浏览器窗口宽度自动缩放，保持 **16:9** 画布、图片比例和内部布局。窗口较矮时可纵向滚动。窄屏会缩小显示整张图，阅读细节时可使用浏览器缩放。

v1.1 的两个文件均内嵌所需素材，也可直接在本地打开。不需要安装、构建、JavaScript 框架、账号或额外下载图片。

## 预览

下方原始 PNG 展示了 v1.1 延续的构图。它是归档的 v1.0 渲染图，并非另行生成的 v1.1 PNG。

![命令与征服及红色警戒社区项目关系图](v1.0/RA-4K.png)

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
| `index.html` | 当前网站入口，与 `v1.1/RA-4K.html` 的文件字节完全一致。 |
| `v1.0/RA-4K.html` | 最初的固定尺寸 HTML。 |
| `v1.0/RA-4K.svg` | 最初的固定尺寸、可编辑 SVG。 |
| `v1.0/RA-4K.png` | 最初的 3840 × 2160 PNG 导出。 |
| `v1.1/RA-4K.html` | 内嵌 SVG 的自适应 HTML。 |
| `v1.1/RA-4K.svg` | 可独立打开的自适应 SVG。 |
| `README.md` / `README.zh-CN.md` | 英文和简体中文项目说明。 |
| `CHANGELOG.md` / `CHANGELOG.zh-CN.md` | 对应的双语版本记录。 |
| `.nojekyll` | 用于 GitHub Pages 直接发布静态文件。 |

已发布的版本目录予以保留。后续功能或内容更新依次放入 **v1.2、v1.3 等新目录**，不覆盖旧版本。网站根目录的 `index.html` 可以随后更新为所选新版本的 HTML，同时更新两份更新日志。

Git 提交和版本目录用于记录发布历史。这个静态网站暂时不需要 GitHub Release，本次 v1.1 发布不创建 Release。

## 后期编辑

重要文字、表格内容、边框和箭头均为可编辑 SVG 元素。可使用 UTF-8 文本编辑器或支持 SVG 的编辑器，修改 SVG 副本或 HTML 内嵌的 SVG。HTML 目前是静态查看页面，不支持直接点击文字编辑或在浏览器内保存修改。

请保留 `0 0 3840 2160` 的 viewBox 和等比缩放设置。修改文字后，检查换行、边界和图片区是否被遮挡。HTML 与 SVG 是独立文件，新版本需要有意识地同步修改两份内容。导出 PNG 时应明确指定 **3840 × 2160**；其他窗口尺寸下的浏览器截图会采用对应窗口尺寸。

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

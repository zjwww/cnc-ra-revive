# cnc-ra-revive

[Live infographic](https://zjwww.github.io/cnc-ra-revive/) · [Changelog](CHANGELOG.md) · [简体中文](README.zh-CN.md)

A visual guide to the relationships between EA's **Command & Conquer / Red Alert** games and **OpenTS, OpenRA, and Chrono Divide**. The infographic combines the original game families, source-code status labels, community development approaches, and a project comparison in one sci-fi RTS layout.

**Current version: v1.2.** The infographic itself uses Simplified Chinese with English game and project names. This English README documents the same artifact; it is not an English translation of the graphic.

## View and zoom

- [Open the HTML website](https://zjwww.github.io/cnc-ra-revive/).
- [Open the latest standalone SVG](https://zjwww.github.io/cnc-ra-revive/RA-4K.svg).

The HTML starts fitted to the window width. Click inside the page if necessary, then use:

| Control | Action |
| --- | --- |
| `Ctrl` + mouse wheel | Zoom the entire infographic around the pointer. |
| `Ctrl` + `+` / `-` | Zoom in / out; `Ctrl` + `=` and numeric-keypad plus/minus are also supported. |
| `Ctrl` + `0` | Restore fit-to-window and return to the top-left corner. |
| Wheel / scrollbars | Move around the enlarged infographic. |

Viewer zoom ranges from 25% to 500% relative to the fitted size. The **16:9** aspect ratio and all module positions stay intact. Resizing the window retains the selected relative zoom; reloading restores fit-to-window.

These HTML shortcuts control **in-page viewer zoom**, not the percentage displayed in the browser's zoom menu. Focus must be in the webpage rather than the address bar or browser menus. The SVG retains browser-native zoom behavior. HTML viewer zoom requires JavaScript; with JavaScript disabled, the graphic still displays fitted to the window.

Both files are self-contained and can also be opened locally. No installation, build step, framework, account, or external image download is required.

## Preview

This 960 × 540 WebP thumbnail is approximately 106 KiB. Click it to open the full viewer. No full-size PNG export is included in the current repository tree.

[![C&C and Red Alert community-project relationship infographic](preview.webp)](https://zjwww.github.io/cnc-ra-revive/)

## What the diagram covers

- Tiberian Dawn, Tiberian Sun, and Firestorm.
- Red Alert, Red Alert 2, and Yuri's Revenge.
- EA's publicly released source repositories and the distinction between engine source and modding resources.
- OpenTS source reconstruction, OpenRA's modernized interpretation, and Chrono Divide's browser-based RA2 approach.
- Colored relationships, source-status labels, and a side-by-side comparison table.

This repository publishes an informational graphic. It does not contain a playable game, an engine implementation, or original game data.

## Files and version preservation

| Path | Purpose |
| --- | --- |
| `index.html` | Latest responsive HTML viewer with whole-graphic zoom controls. |
| `RA-4K.svg` | Latest responsive, editable standalone SVG. |
| `preview.webp` | Small thumbnail for the READMEs. |
| `README.md` / `README.zh-CN.md` | English and Simplified Chinese project documentation. |
| `CHANGELOG.md` / `CHANGELOG.zh-CN.md` | Matching version histories. |
| `.nojekyll` | Direct static-file publishing on GitHub Pages. |

The current GitHub tree contains only the latest HTML and SVG, the small preview, documentation, and repository configuration. It has no `v1.0` / `v1.1` directories or full-size PNG export. Older files remain available in earlier Git commits; Git history has not been rewritten.

Local working copies keep each version separately as **v1.0, v1.1, v1.2, v1.3, and so on**. Future updates preserve those local archives, replace the current root files on GitHub, and update both changelogs. GitHub Releases are not used for this static site.

## Editing

Important text, table entries, borders, and arrows are editable SVG elements. Edit a copy of the SVG or the inline SVG inside the HTML with a UTF-8 text editor or an SVG-capable editor. The HTML is a static viewer; it does not offer click-to-edit controls or in-browser saving.

Keep the `0 0 3840 2160` viewBox, proportional scaling rules, and viewer controls. When changing copy, check wrapping, text boundaries, and image separation. The HTML and SVG are separate files: update both copies deliberately for a new version. To export a PNG, render at **3840 × 2160** explicitly; a browser screenshot at another window size will have that window's dimensions.

## Scope and visual limitations

The content is an editorial snapshot prepared in September 2026, not a live status monitor or a complete technical audit. Strong labels such as “original source code lost” are inherited from the supplied infographic brief; this repository does not independently establish those historical claims. Lack of a public source release alone does not prove that all original source copies are lost. Fidelity ratings are qualitative, and compatibility can change.

Backgrounds, game-style illustrations, and emblems include AI-generated reconstructions and may differ from official artwork. Text and diagram geometry were rendered on a 3840 × 2160 canvas, but the decorative raster source was 1672 × 941; the artwork is **not entirely native 4K**. The complete infographic was rebuilt rather than simply enlarging the supplied reference. Typography uses system fonts, primarily Microsoft YaHei and Arial, so rendering can differ on systems without those fonts.

The self-contained HTML and SVG are each approximately 10 MB because images are embedded. A later version could share and optimize image assets to improve loading speed while retaining the archived files.

## Upstream references

Use upstream documentation for current project status and technical details:

- [EA: CnC_Tiberian_Dawn](https://github.com/electronicarts/CnC_Tiberian_Dawn) — official public source repository.
- [OpenTS](https://github.com/OpenTS-Developers/OpenTS) — Tiberian Sun reconstruction project and documentation.
- [About OpenRA](https://www.openra.net/about/) — project goals and modernized gameplay.
- [Chrono Divide](https://chronodivide.com/) — browser-based Red Alert 2 project.
- [Chrono Divide Mod SDK](https://github.com/chronodivide/mod-sdk) — modding compatibility and limitations.

## Hosting

GitHub Pages publishes the `main` branch from the repository root. `index.html` opens the infographic on the website; `README.md` remains the default project description on GitHub. The `.nojekyll` file disables Jekyll processing. See [GitHub's Pages setup documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site).

## Attribution and licensing

This is an independent community infographic and is not affiliated with or endorsed by Electronic Arts, OpenTS, OpenRA, or Chrono Divide. Game names, trademarks, project names, and third-party visual identities are acknowledged as belonging to their respective owners.

No project-wide redistribution license has been selected for this repository. Public availability should not be interpreted as a blanket license for third-party artwork or marks. The upstream projects have their own licenses; those licenses do not automatically apply to this infographic.

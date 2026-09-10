# cnc-ra-revive

[Changelog](CHANGELOG.md) · [简体中文](README.zh-CN.md) · [Published site](https://zjwww.github.io/cnc-ra-revive/)

A visual guide to EA's **Command & Conquer / Red Alert** games and **OpenTS, OpenRA, and Chrono Divide**.

**Current version: v1.8.** The default website uses browser-native zoom. Four self-contained files offer two zoom mechanisms. Every file preserves the same 3840 × 2160 coordinate system, 16:9 artwork proportions, 177 text elements, and fixed internal layout.

## Open a version

| Mechanism | HTML | Standalone SVG |
| --- | --- | --- |
| Browser-native zoom | [index.html](https://zjwww.github.io/cnc-ra-revive/index.html) | [RA-4K.svg](https://zjwww.github.io/cnc-ra-revive/RA-4K.svg) |
| In-page code zoom | [RA-4K-viewer.html](https://zjwww.github.io/cnc-ra-revive/RA-4K-viewer.html) | [RA-4K-viewer.svg](https://zjwww.github.io/cnc-ra-revive/RA-4K-viewer.svg) |

Open each SVG directly in a browser tab for its interactive behavior. Each HTML and SVG includes its own artwork and script, so none requires a neighboring file or network connection. The two formats in each pair use identical viewer code.

## iPhone / touch browsing

All four files delegate pinch zoom and panning to the mobile browser. The in-page pair retains its code-driven wheel/keyboard controls on desktop only. Mobile tab titles say “手机浏览器手势缩放”; they do not report a misleading in-page percentage.

The first fit uses stable small-viewport CSS width (`svw`) where supported; stable height (`svh`) also participates in rotation-settling checks. Pinch zoom, panning and toolbar-only height changes do not rewrite the artwork size. A rotation or genuine layout-width change is fitted after about 150 ms of stable measurements and two animation-frame checks. Differences within one CSS pixel are ignored. An 800 ms deadline abandons an unsettled attempt; it never forces a fit during an active touch gesture. Subsequent relevant events can start a new attempt.

No mobile touch/gesture default is cancelled, browser zoom is not reset, and the script never calls `scrollTo()` on mobile. Rotation does not promise to preserve an exact image coordinate: Safari controls its own zoom and scroll restoration. A stable new orientation may change the fitted size once. Without small-viewport unit support, fitting is conservatively limited to initial load and orientation changes.

The v1.7 mobile candidate was tested by the user on the reported iPhone 14 Pro / iOS 26.6.2 without further issues. v1.8 retains that gesture policy and changes the fit to use width. Automated desktop/mobile emulation checks do not replace real-device testing of this new fit. The graphic, arrow fixes and 16:9 coordinates are unchanged.

## Desktop zoom behavior

| Action | Native pair | In-page pair |
| --- | --- | --- |
| Ctrl + wheel, Ctrl + plus/minus | Browser handles zoom; its menu percentage changes. | Code zooms the artwork from 25% to 500%; browser percentage stays unchanged. |
| Ctrl + 0 | Browser returns to 100%. | Restore width-fitted artwork and scroll to the top-left. |
| Percentage display | Browser zoom menu. | Tab title, for example “页面内缩放 150%”. |
| Resize window | Adapt the fitted reference while retaining relative native zoom. | Adapt the fit while retaining the selected in-page multiplier. |
| Reload | Keep the native fitted reference when session storage is available. | Reset in-page zoom to the fitted size. |

All four files initially **fit the available viewport width**. Height follows at 9/16 of the artwork width; a shorter window uses vertical scrolling. The artwork is never stretched, cropped or rearranged. Desktop zoom enlarges or reduces this width-fit reference; after enlargement, use ordinary scrolling to reach the rest of the graphic. Mobile pinch zoom remains controlled by the browser.

### Native fit reference

The native pair leaves wheel and keyboard defaults intact. A small script calculates proportional dimensions; it does not set or simulate the browser's zoom percentage. The first visit in a tab establishes a fit reference at the browser's **current** zoom and display scaling. Session storage retains this reference through reloads, where supported.

For comparable baseline testing, set the browser to **100% before opening each file in a fresh tab**. Opening a fresh tab for the first time at 150% fits the image at that initial 150%; this is intentionally different from opening at 100% and then enlarging to 150%. Ctrl + 0 always resets browser zoom, but does not redefine the stored fit reference. If session storage is blocked, reloading establishes a new reference. Moving between monitors with different display scaling has not been verified; use a fresh tab to establish a new reference there.

### In-page controls and compatibility

Focus the document before using shortcuts. Ctrl + equals and numeric-keypad plus/minus are also supported. Wheel zoom retains the point under the pointer where scrolling bounds allow; keyboard zoom uses the viewport center. The title displays the in-page multiplier, not browser zoom. Changing zoom directly in the browser menu remains a separate browser operation.

JavaScript is required for the shared sizing behavior and in-page controls. SVG scripts run when opened as an interactive document; embedding an SVG using an HTML image element disables its scripts, so it becomes a static image. The graphic remains editable SVG text and imagery in every file.

## Preview

[![Infographic preview](preview.webp)](https://zjwww.github.io/cnc-ra-revive/index.html)

The small 960 × 540 WebP is documentation-only.

## What the diagram covers

- Tiberian Dawn, Tiberian Sun, and Firestorm.
- Red Alert, Red Alert 2, and Yuri's Revenge.
- EA's publicly released source repositories and the distinction between engine source and modding resources.
- OpenTS source reconstruction, OpenRA's modernized interpretation, and Chrono Divide's browser-based RA2 approach.
- Colored relationships, source-status labels, and a side-by-side comparison table.

This repository publishes an informational graphic. It does not contain a playable game, an engine implementation, or original game data.

## Files and version preservation

The current version contains four viewers: `index.html`, `RA-4K.svg`, `RA-4K-viewer.html`, and `RA-4K-viewer.svg`. A small WebP preview and separate English/Chinese documentation are included. Historical version directories are kept out of the current GitHub tree.

## Editing

Important text, table entries, borders, and arrows are editable SVG elements. Edit a copy of the SVG or the inline SVG inside the HTML with a UTF-8 text editor or an SVG-capable editor. The HTML is a static viewer; it does not offer click-to-edit controls or in-browser saving.

Keep the `0 0 3840 2160` viewBox, proportional scaling rules, and viewer controls. When changing copy, check wrapping, text boundaries, and image separation. The HTML and SVG are separate files: update both copies deliberately for a new version. To export a PNG, render at **3840 × 2160** explicitly; a browser screenshot at another window size will have that window's dimensions.

## Scope and visual limitations

The content is an editorial snapshot prepared in September 2026, not a live status monitor or a complete technical audit. Strong labels such as “original source code lost” are inherited from the supplied infographic brief; this repository does not independently establish those historical claims. Lack of a public source release alone does not prove that all original source copies are lost. Fidelity ratings are qualitative, and compatibility can change.

Backgrounds, game-style illustrations, and emblems include AI-generated reconstructions and may differ from official artwork. Text and diagram geometry were rendered on a 3840 × 2160 canvas, but the decorative raster source was 1672 × 941; the artwork is **not entirely native 4K**. The complete infographic was rebuilt rather than simply enlarging the supplied reference. Typography uses system fonts, primarily Microsoft YaHei and Arial, so rendering can differ on systems without those fonts.

The self-contained HTML and SVG are each approximately 10 MB because images are embedded.

## Upstream references

Use upstream documentation for current project status and technical details:

- [EA: CnC_Tiberian_Dawn](https://github.com/electronicarts/CnC_Tiberian_Dawn) — official public source repository.
- [OpenTS](https://github.com/OpenTS-Developers/OpenTS) — Tiberian Sun reconstruction project and documentation.
- [About OpenRA](https://www.openra.net/about/) — project goals and modernized gameplay.
- [Chrono Divide](https://chronodivide.com/) — browser-based Red Alert 2 project.
- [Chrono Divide Mod SDK](https://github.com/chronodivide/mod-sdk) — modding compatibility and limitations.

## Hosting

GitHub Pages serves the browser-native HTML as its homepage. The other three viewers are available through the links above.

## Attribution and licensing

This is an independent community infographic and is not affiliated with or endorsed by Electronic Arts, OpenTS, OpenRA, or Chrono Divide. Game names, trademarks, project names, and third-party visual identities are acknowledged as belonging to their respective owners.

No project-wide redistribution license has been selected for this repository. Public availability should not be interpreted as a blanket license for third-party artwork or marks. The upstream projects have their own licenses; those licenses do not automatically apply to this infographic.

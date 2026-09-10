# Changelog

[README](README.md) · [简体中文更新日志](CHANGELOG.zh-CN.md) · [简体中文说明](README.zh-CN.md) · [Live infographic](https://zjwww.github.io/cnc-ra-revive/)

Versions describe this infographic and its viewer, not the release versions of the games or community engines shown in it. Local versions are archived separately. From v1.2 onward, the current GitHub tree contains only the latest artifacts. Previously published versions remain in Git history; v1.3 and v1.4 were local-only candidates.

## v1.5 — 2026-09-10

- Added native HTML/SVG and in-page HTML/SVG: four independent, self-contained files.
- Used identical sizing and interaction code for both formats in each pair, with a fixed 3840 × 2160 viewBox and one uniform scale. Preserved all original artwork, coordinates, and 177 text elements.
- Native mode delegates zoom input to the browser and uses session storage to retain the initial fit reference on reload. The initial browser zoom establishes that reference; it is not assumed to be 100%.
- In-page mode handles Ctrl + wheel, plus/minus and zero; supports 25%–500%, pointer anchoring, window resizing, and a percentage in the tab title. Browser zoom percentage remains separate.
- Published after user testing and approval. The native HTML viewer is the Pages homepage (`index.html`); the native SVG keeps its original `RA-4K.svg` URL. The alternate pair uses `RA-4K-viewer.html` and `RA-4K-viewer.svg`.
- Preserved all local v1.0–v1.5 archives. The GitHub root contains only the latest four viewers, thumbnail, documentation, and configuration. No GitHub Release was created.
- See README for initialization, script restrictions, and cross-monitor validation limits.

### Validation

- Microsoft Edge: 96 recorded checkpoints across all four files at 100% and 150% display scaling. Verified actual native zoom at 80%, 100%, 110%, 150%, and 200%, reload retention, window resizing, and access to the right/bottom edges.
- Exercised in-page keyboard and Ctrl + wheel events, 25%/500% limits, reset, title percentage, and unchanged browser DPR. Native shortcut handlers were checked to leave default actions uncancelled; native rendering was exercised through Edge's zoom setting rather than physical keyboard input.
- Fresh 150% native openings and reloads matched the documented initial-fit behavior in HTML and SVG, both locally and over a temporary localhost HTTP server. Also checked both HTTP in-page viewers. No public deployment was used.

## v1.4 — Local candidate, not published

### Fixed

- Replaced the standalone SVG root's automatic height with `100%` in both its attribute and CSS. The complete graphic now fits the available window at 100% browser zoom, and native zoom actually enlarges or reduces the artwork and text.
- Retained top-left alignment and uniform scaling. All 177 text elements, artwork, and internal geometry are unchanged. No scripts or shortcut handlers were added to the SVG.
- Kept the HTML and thumbnail byte-identical to v1.2. Preserved all previous local versions and the published repository working copy.

### Validation and publication status

- Reproduced v1.3's enlargement failure: at 150% browser zoom, actual artwork and text remained approximately 100% of their original displayed size. The earlier v1.3 checks measured alignment and proportionality but missed this failure.
- Changed native Edge zoom on the same open document in an isolated test profile through 110%, 125%, 150%, 200%, 80%, 50%, and back to 100%. Verified actual artwork and text size against each zoom factor, zero origin drift, and equal X/Y scaling.
- Verified scrolling to the right and bottom edges at 200%, window resizing, and both 100% and 150% display scaling. These automated checks change Edge's native zoom setting; physical mouse-wheel and keyboard operation remains for user confirmation.
- Local only: no commit, push, or GitHub Pages deployment. Awaiting user testing and explicit publication approval.

## v1.3 — Local candidate, not published; superseded by v1.4

Known limitation: this candidate removed the left gutter but did not fix actual enlargement above 100%. Its fixes were carried forward into v1.5.

### Fixed

- Changed only the standalone SVG root alignment from `xMidYMin meet` to `xMinYMin meet`, removing the expanding left gutter when using native browser zoom above 100%.
- Preserved proportional scaling, all 177 text elements, and all artwork and internal geometry. The HTML and preview are unchanged copies of v1.2.

### Validation and publication status

- Reproduced the old left gutter using actual native page-zoom preferences in isolated Microsoft Edge test profiles.
- Compared v1.2 and v1.3 at 80%, 100%, 110%, 125%, 150%, and 200%. The candidate keeps the left-origin offset at zero and equal X/Y scaling at every level.
- Local candidate only: no Git commit, push, or Pages deployment. Awaiting user testing and explicit publication approval.

## v1.2 — 2026-09-10

### Changed

- Added whole-infographic zoom in HTML: Ctrl + wheel, Ctrl + plus/minus (including the numeric keypad), and Ctrl + 0 to restore fit-to-window.
- Kept the layout proportional while zooming from 25% to 500%; added pointer anchoring for wheel zoom and a scrollable viewport for enlarged content.
- Preserved relative zoom when resizing the window and restored fit-to-window on reload. These controls adjust the in-page viewer, not the browser's zoom percentage.
- Preserved standalone SVG behavior and all 177 text elements and artwork geometry.
- Flattened the published repository to the latest `index.html` and `RA-4K.svg`. Removed version directories and the full-size PNG from the current tree without rewriting history or deleting local archives.
- Added a 960 × 540 WebP README thumbnail of approximately 106 KiB.
- Changed the English README language link to “简体中文” and synchronized both READMEs and changelogs, including historical links.

### Validation

- Checked keyboard and mouse zoom, reset, pointer anchoring, scrolling, window resizing, range limits, and five fitted viewport sizes in Microsoft Edge.
- Verified that original local v1.0/v1.1 files and the standalone SVG remain unchanged.

## [v1.1](https://github.com/zjwww/cnc-ra-revive/blob/046f4957a5c2baacc75b7e6c28c625633117c319/v1.1/RA-4K.html) — 2026-09-10

### Changed

- Made the HTML viewer responsive on 2026-09-07: the complete composition scales with the browser width, preserving its 16:9 aspect ratio and module positions.
- Added responsive standalone SVG on 2026-09-10, preserving the original 3840 × 2160 viewBox, text, artwork, and diagram geometry.
- Retained vertical scrolling for windows shorter than the scaled composition.

### Publication

- Prepared the first GitHub publication as `cnc-ra-revive`, with v1.1 as the website entry point.
- Added paired English and Simplified Chinese READMEs and changelogs with navigation links.
- Configured direct static publishing from `main` using GitHub Pages and `.nojekyll`.
- Included the original v1.0 HTML, SVG, and PNG archive, without changing their file contents.
- Kept v1.1 HTML and SVG unchanged during publication; `index.html` duplicates the versioned HTML exactly.
- Did not create a GitHub Release. Git commits and preserved directories track the published artifacts.

### Validation

- Checked the HTML and SVG at viewport sizes of 3840 × 2160, 1920 × 1080, 1280 × 800, 1000 × 450, and 390 × 844 in Microsoft Edge.
- Confirmed equal horizontal and vertical scaling, no horizontal overflow, and preservation of all 177 text elements.
- Verified archived file hashes before publication.

## [v1.0](https://github.com/zjwww/cnc-ra-revive/blob/046f4957a5c2baacc75b7e6c28c625633117c319/v1.0/RA-4K.html) — 2026-09-06

### Added

- Original 3840 × 2160 infographic in PNG, editable SVG, and fixed-size HTML formats.
- Official game families on the left, relationships in the center, community projects on the right, and a comparison table and legend at the bottom.
- Rebuilt text, borders, arrows, and table geometry over generated sci-fi artwork.

### Known limitations

- Decorative raster artwork is not native 4K, despite the 4K canvas and export dimensions.
- The original fixed-size HTML does not automatically fit narrower browser windows.
- Source-status and compatibility descriptions are an editorial snapshot; see the README for scope and upstream references.

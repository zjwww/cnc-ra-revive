# Changelog

[README](README.md) · [简体中文更新日志](CHANGELOG.zh-CN.md) · [简体中文说明](README.zh-CN.md) · [Live infographic](https://zjwww.github.io/cnc-ra-revive/)

Versions describe this infographic and its viewer, not the release versions of the games or community engines shown in it. Local versions are archived separately. From v1.2 onward, the current GitHub tree contains only the latest artifacts; earlier versions remain in Git history.

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

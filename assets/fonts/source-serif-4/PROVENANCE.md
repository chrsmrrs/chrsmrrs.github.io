# Source Serif 4 webfont provenance

Retrieved 2026-09-25 from official Google Fonts and Adobe sources. Font binaries are downloaded byte-for-byte; no font conversion, instancing, subsetting, metadata edits, or system-font installation was performed.

## Source requests

- Google Fonts CSS request: https://fonts.googleapis.com/css2?family=Source+Serif+4:opsz,wght@8..60,400&display=swap
- User agent: `Mozilla/5.0 AppleWebKit/537.36 (KHTML, like Gecko) Chrome/130.0.0.0 Safari/537.36`
- Original response: `google-fonts-original.css` (all official subset declarations, unchanged).
- Latin WOFF2: https://fonts.gstatic.com/s/sourceserif4/v14/vEFF2_tTDB4M7-auWDN0ahZJW3IX2iZPwg3BucvUtfykDXr4.woff2
- Latin Extended WOFF2: https://fonts.gstatic.com/s/sourceserif4/v14/vEFF2_tTDB4M7-auWDN0ahZJW3IX2iZPwg3BucvUtfykA3r4cXk.woff2
- Google Fonts original license (`OFL.txt`): https://raw.githubusercontent.com/google/fonts/main/ofl/sourceserif4/OFL.txt
- Matching Adobe 4.004 release license (`ADOBE-LICENSE.md`): https://raw.githubusercontent.com/adobe-fonts/source-serif/4.004R/LICENSE.md
- Adobe source project: https://github.com/adobe-fonts/source-serif

## Files and verification

| Filename | Size | SHA-256 |
| --- | ---: | --- |
| source-serif-4-latin-400-normal.woff2 | 48,596 bytes | ba627ffc66e406b09078e06d4a683a6f4dec989b258927ce8f165d046e23bf2f |
| source-serif-4-latin-ext-400-normal.woff2 | 40,928 bytes | b2c5fe7ba18277496af5e074d9035e98f679ab021bdc41e3456de97c305ffdcb |

Both files decode successfully as WOFF2 TrueType fonts, and every font table was decompiled with fontTools 4.57.0. Embedded family `Source Serif 4`, subfamily `Regular`, PostScript name `SourceSerif4-Regular`, version `4.004`, OS/2 weight 400, italic flag false. Each file has only the `opsz` variation axis: minimum 8, default 20, maximum 60. They have fixed weight 400; neither is a weight-variable file.

Character-map inspection confirms Latin has `ÄÖÜäöüß` and common French/Western European accents; Latin Extended adds capital `ẞ` and accented Latin such as `ŁłŠšŽžČčĞğİŐőŰű`. All characters in the combined sample below are mapped across the two files:

`ÄÖÜäöüßẞéèêëàáâãåæçìíîïñòóôõøùúûÿœŁłŠšŽžČčĞğİıŐőŰű`

Detailed results and hashes: `verification.json`. This is actual cmap coverage, not just claimed CSS ranges. Google CSS ranges are broad loading declarations, not a guarantee of every codepoint in each range.

## Self-hosting CSS

Use `self-host-example.css`, adjusting only the file URL paths for the site's asset location. It includes the original Google `unicode-range` declarations for these two files and declares `font-style: normal`, `font-weight: 400`, and `font-display: swap`.

For styled elements, set `font-family: 'Source Serif 4', serif; font-weight: 400; font-optical-sizing: auto;`. Optical sizing uses the original font's `opsz` axis. Keep both original license files with redistributed font assets: the matching Adobe release license retains the copyright and Reserved Font Name notice also found inside the binaries.

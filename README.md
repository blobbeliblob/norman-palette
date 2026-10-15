# Norman

[Open the Norman palette website](https://blobbeliblob.github.io/norman-palette/)

**A geometric UI color palette with a little humanity.** Norman is a dark-first palette for Noctalia, built around near-black surfaces, soft neutrals, and a few expressive accents.

## Noctalia

The palette is available as [`Norman.json`](Norman.json) and [`Norman Muted.json`](Norman%20Muted.json). The GitHub Pages preview can switch between the normal and muted palettes.

## Main palette

HEX values are written with a leading `#`. HSL uses degrees for hue and percentages for saturation and lightness; components are rounded to the nearest 5.

| Color | Use | HEX | HSL |
| --- | --- | --- | --- |
| Surface | Background, base surface — black, with the tiniest hint of humanity | `#0D0D0D` | `hsl(0 0% 5%)` |
| On surface | Main foreground — white, with corruption seething | `#F2F2F2` | `hsl(0 0% 95%)` |
| Surface variant | Raised and alternate surfaces | `#333333` | `hsl(0 0% 20%)` |
| Outline | Borders and dividers — between good and evil | `#808080` | `hsl(0 0% 50%)` |
| Shadow | Dark elevation and depth | `#4D4D4D` | `hsl(0 0% 30%)` |
| Primary | Green, drifting out to the sea | `#33CC99` | `hsl(160 60% 50%)` |
| Secondary | Yellow, like the king | `#F0DB75` | `hsl(50 80% 70%)` |
| Tertiary | Rose, full of charm | `#F0758A` | `hsl(350 80% 70%)` |
| Hover | Soft mint interaction state | `#ADEBD6` | `hsl(160 60% 80%)` |
| Error | Error and destructive states | `#F07575` | `hsl(0 80% 70%)` |

## Light surfaces

The accent colors remain consistent between themes. These surface roles change in the light variant:

| Color | Use | HEX | HSL |
| --- | --- | --- | --- |
| Surface | Background, base surface | `#F2F2F2` | `hsl(0 0% 95%)` |
| On surface | Main foreground | `#0D0D0D` | `hsl(0 0% 5%)` |
| Surface variant | Raised and alternate surfaces | `#CCCCCC` | `hsl(0 0% 80%)` |
| Shadow | Light elevation and depth | `#B3B3B3` | `hsl(0 0% 70%)` |

## Terminal colors

| Color | Normal | Bright |
| --- | --- | --- |
| Black | `#0D0D0D` · `hsl(0 0% 5%)` | `#4D4D4D` · `hsl(0 0% 30%)` |
| Red | `#BF5540` · `hsl(10 50% 50%)` | `#E6BBB3` · `hsl(10 50% 80%)` |
| Green | `#40BF55` · `hsl(130 50% 50%)` | `#B3E6BB` · `hsl(130 50% 80%)` |
| Yellow | `#BFAA40` · `hsl(50 50% 50%)` | `#E6DDB3` · `hsl(50 50% 80%)` |
| Blue | `#4055BF` · `hsl(230 50% 50%)` | `#B3BBE6` · `hsl(230 50% 80%)` |
| Magenta | `#BF40AA` · `hsl(310 50% 50%)` | `#E6B3DD` · `hsl(310 50% 80%)` |
| Cyan | `#66CCCC` · `hsl(180 50% 60%)` | `#B3DDE6` · `hsl(190 50% 80%)` |
| White | `#F2F2F2` · `hsl(0 0% 95%)` | `#B3B3B3` · `hsl(0 0% 70%)` |

| Terminal role | HEX | HSL |
| --- | --- | --- |
| Background | `#0D0D0D` | `hsl(0 0% 5%)` |
| Foreground | `#F2F2F2` | `hsl(0 0% 95%)` |
| Cursor | `#33CC99` | `hsl(160 60% 50%)` |
| Cursor text | `#B3E6D5` | `hsl(160 50% 80%)` |
| Selection background | `#D9F2EA` | `hsl(160 50% 90%)` |
| Selection foreground | `#0D261E` | `hsl(160 50% 10%)` |

## Muted palette

These are the muted dark-theme UI colors shown when the preview's **Muted** toggle is on:

| Color | HEX | HSL |
| --- | --- | --- |
| Surface | `#262626` | `hsl(0 0% 15%)` |
| On surface | `#CCCCCC` | `hsl(0 0% 80%)` |
| Surface variant | `#404040` | `hsl(0 0% 25%)` |
| Outline | `#808080` | `hsl(0 0% 50%)` |
| Shadow | `#595959` | `hsl(0 0% 35%)` |
| Primary | `#4DB391` | `hsl(160 40% 50%)` |
| Secondary | `#D9CC8C` | `hsl(50 50% 70%)` |
| Tertiary | `#D98C99` | `hsl(350 50% 70%)` |
| Hover | `#70C2A7` | `hsl(160 40% 60%)` |
| Error | `#D98C8C` | `hsl(0 50% 70%)` |

## JSON schema

Both palette files use the same structure. Each file has top-level `dark` and `light` themes. Every theme contains these UI color tokens:

`mPrimary`, `mOnPrimary`, `mSecondary`, `mOnSecondary`, `mTertiary`, `mOnTertiary`, `mError`, `mOnError`, `mSurface`, `mOnSurface`, `mSurfaceVariant`, `mOnSurfaceVariant`, `mOutline`, `mShadow`, `mHover`, and `mOnHover`.

Each theme also contains a `terminal` object with `background`, `foreground`, `cursor`, `cursorText`, `selectionBg`, `selectionFg`, `normal`, and `bright`. The `normal` and `bright` objects each define `black`, `red`, `green`, `yellow`, `blue`, `magenta`, `cyan`, and `white`. All color values are `#RRGGBB` strings.

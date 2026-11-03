# Smalt brand assets

The mark is four squares on the 32-unit grid the favicon has always used —
inset 5, square 10, gap 2 — with the fourth square in smalt, the blue pigment
the product is named after. The wordmark is IBM Plex Sans at **wght 400**
(non-bold), set at a font size equal to the mark's 22-unit block, which puts
its cap height at 70 % of the mark. The glyphs are outlines in the SVGs, so
nothing here needs a webfont.

The name is set in the pigment, not in the neutral — the same way the site
header sets it — so each lockup carries one blue: `#5f90ea` for the name and
the accent square on the ink ground, `#003399` for both on a light one. The
three remaining squares stay neutral.

## The two blues

| Token | Value | Use |
| --- | --- | --- |
| `--smalt` | `#003399` | the pigment itself — light grounds |
| `--smalt-light` | `oklch(0.66 0.145 262)` → `#5f90ea` | the same hue lifted for dark grounds, where `#003399` falls to 1.7:1 |

Neutrals are `#161616` (`--ink`) and `#f4f4f3` (`--color-bg`).

## Files

| File | What it is |
| --- | --- |
| `smalt-mark.svg` | mark alone, no name, on the ink ground |
| `smalt-mark-on-light.svg` | mark alone, transparent ground, ink squares + `#003399` |
| `smalt-logo.svg` | mark + the name in `#5f90ea`, on the ink ground |
| `smalt-logo-on-light.svg` | mark + the name in `#003399`, transparent ground |
| `smalt-mark-512.png`, `smalt-mark-on-light-512.png` | raster mark, 512 × 512 |
| `smalt-logo-512.png`, `smalt-logo-on-light-512.png` | raster lockup, 512 tall |
| `icon-32.png`, `icon-180.png`, `icon-192.png`, `icon-512.png` | icons on the ink ground — 180 is the Apple touch icon, 192/512 are the PWA sizes, and 512 doubles as the GitHub social preview |
| `../favicon.ico` | 16/32/48 frames of the same mark |

Prefer the SVGs anywhere they are allowed: they stay sharp and carry no font
dependency. The `-on-light` files have a transparent ground, so they sit on
white, on `#f4f4f3`, or on any pale surface.

Clearspace is built in: the 5-unit inset around the mark (and to the right of
the name) is the minimum — keep at least that much, measured in units of the
mark's own square, between the logo and anything else.

Do not re-colour the squares or the name, re-set the name in another family or
weight, or pull the mark and the name apart into a new arrangement. If you need a
different size, scale the SVG.

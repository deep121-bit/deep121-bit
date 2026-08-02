# Design Notes

## Color Palette

| Role | Hex | Usage |
|---|---|---|
| Background | `#0D1117` | Banner base, terminal windows, cards |
| Primary (Purple) | `#7C3AED` | Gradients, borders, primary button |
| Secondary (Cyan) | `#00E5FF` | Scanner sweeps, glow rings, accents |
| Accent (Pink) | `#FF4D8D` | Gradient end, highlights |
| Text | `#FFFFFF` | Headings, names |
| Secondary Text | `#B0BEC5` | Body copy, meta lines |

`banner-light.svg` swaps the background to white/lavender (`#FFFFFF` → `#F5F3FF`) and darkens body text
to `#4B5563` while keeping the purple/cyan/pink accents — they read fine on both themes.

## Animation Inventory

| File | Effect |
|---|---|
| `assets/images/banner.svg` / `banner-light.svg` | Terminal typing, gradient name reveal, cycling role titles, tech pills, avatar hologram, buttons, scanner sweep |
| `assets/images/background.svg` | Tileable grid + drifting particles, used as a section divider |
| `assets/animations/terminal.svg` | Standalone terminal window with multi-line typing sequence |
| `assets/animations/hologram.svg` | Reusable scan-line + flicker overlay — drop over any circular avatar |
| `assets/animations/particles.svg` | Transparent floating-dot overlay, layer above any banner |
| `assets/animations/lanyard.svg` | Drop-in + damped pendulum swing + holographic card shine |

All animations use only **SMIL (`<animate>`, `<animateTransform>`) and SVG-native effects** — no JavaScript,
since GitHub strips `<script>` tags from README-rendered SVGs.

## Cache Busting

GitHub aggressively caches images embedded in READMEs. Every local asset reference carries a `?v=N`
query string; bump the number (or let `profile-update.yml` do it weekly) whenever you edit an SVG and
want GitHub to actually show the new version.

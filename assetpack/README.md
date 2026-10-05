# Cthulhu Runner — 2D Pixel Art Asset Pack (Lovecraftian Horror)

A Lovecraftian-horror themed 2D pixel art asset pack for side-view
platformer/runner games. All sprites are PNG with alpha transparency
(except backgrounds), generated at a chunky 16-bit style and downscaled
to crisp pixel resolution.

## Contents

```
assetpack/pixelart/
├── characters/
│   └── hero_sheet.png        # 1920s occult investigator: idle + walk/run frames (256×192)
├── enemies/
│   └── enemies_sheet.png      # Deep One, cultist, tentacled horror — anim strips (256×192)
├── tilesets/
│   └── tileset.png           # Stone brick, cracked stone, mossy rock, wood, rune tiles (256×192)
├── props/
│   └── props_sheet.png       # Tomes, amulet, lantern, skull, dagger, crate, barrel… (256×192)
└── backgrounds/
    ├── bg_sky.png            # Night sky, moon, stars, village silhouette (256×64)
    ├── bg_cliffs.png         # Rocky cliffs with dead trees — parallax layer (256×64)
    └── bg_fog.png            # Foreground fog layer (256×64)
```

## Style

- Dark Lovecraftian palette: muted teals, sickly greens, sepia browns, deep blacks.
- 16-bit era inspired pixel art, nearest-neighbor downscaled ×4 for crisp pixels.
- Transparent backgrounds on all sprites (chroma-key + flood-fill removal).
- Backgrounds are designed as horizontal parallax layers; tile horizontally
  (wrap the seam or mirror) for endless scrolling.

## Usage notes

- **Sheets are 256×192 reference rasters**, not strict uniform grids — slice
  sprites by their alpha bounding boxes, or use them directly as decoration sheets.
- Backgrounds are 256×64 strips; scale to your target resolution with
  nearest-neighbor sampling to preserve hard pixel edges.
- Suggested tile size for the tileset: 16×16 or 32×32 cells, slice to taste.

## License

CC0 1.0 Universal (Public Domain Dedication). Free for commercial and
personal use, no attribution required (but appreciated!).

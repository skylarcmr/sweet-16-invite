# Simone Sweet 16 — Figma Export

## Files

| File | What | Edit in Figma |
|---|---|---|
| `01_closed_envelope.svg` | Closed envelope with seal | Layers: env-back, env-front, env-flap, env-seal |
| `02_open_envelope.svg` | Envelope with flap rotated up | Layers: env-flap-open, env-back, env-front |
| `03_balloons.svg` | 16 balloons in 2 rows (color reference) | Each balloon is its own group |
| `04_full_scene.svg` | Complete scene — stage bg + envelope + balloons | Top-level groups: stage-bg, balloons, envelope |
| `seal.png` | Wax seal asset (transparent PNG) | Re-import as image fill |
| `card_front.jpg` | Pre-rendered Sweet 16 invite (existing asset) | The card face |

## Color tokens

```
Hot pink       #e8175d
Hot pink dark  #b50e48
Light pink     #f9d6e7
Cream          #fce8f0
Stage dark     #0d0d0d  ← page bg
Stage glow     #2a1820  ← bg radial center
Knot dark      #8b0a35
```

## Balloon palette (5 gradients)

| Name | Highlight → Mid → Deep |
|---|---|
| `grad_hotpink`   | #ffc4d8 → #ff5a99 → #e8175d → #8b0a35 |
| `grad_lightpink` | #ffe6f0 → #ffb3cc → #ff8aaf → #c75a85 |
| `grad_magenta`   | #ffb0e0 → #ff3399 → #c80f6f → #5a042f |
| `grad_black`     | #9a9a9a → #3a3a3a → #161616 → #000 |
| `grad_gold`      | #fff4cf → #f3d27a → #c89c2e → #7a5a10 |

## Geometry reference

- Envelope: 360 × 240 (desktop), 85vw × 0.66·85vw (mobile)
- Flap closed: triangle pointing down to `(50%, 48%)`
- Flap open: same triangle rotated 180° around top edge
- Seal: 90 × 90, centered on flap point (50%, 48%)
- Balloons spawn at envelope top (50% – 100px), drift up & out

## How to import

1. Drag any `.svg` into Figma — it preserves vectors and layer names
2. For the full scene, start with `04_full_scene.svg` and break apart groups
3. Replace `card_front.jpg` reference with whatever invite design you finalize

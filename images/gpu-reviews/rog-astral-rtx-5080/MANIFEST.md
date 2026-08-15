# ROG Astral RTX 5080 OC — Image & Video Asset Manifest

**Captured by:** LK Wood IV, St. Louis County MO (operator's primary rig)
**Processed:** 2026-06-13 by COA
**Source files:** Operator's iPhone (IMG_1689–IMG_1698), shot at 4032×3024 / 4K30 HEVC
**Output:** All metadata stripped (EXIF, GPS, device info). Hugo-friendly slugs. Responsive srcset variants.

## Directory layout

```
static/images/gpu-reviews/rog-astral-rtx-5080/
  {slug}-1600.webp    # hero, modern browsers
  {slug}-1600.jpg     # hero, fallback
  {slug}-800.webp     # mobile + responsive srcset
  {slug}-800.jpg      # mobile fallback
  {slug}-400.webp     # thumbnail / open-graph

static/videos/gpu-reviews/rog-astral-rtx-5080/
  rog-astral-5080-rgb-cycle-1080.mp4    # H.264, ~6.9MB, desktop
  rog-astral-5080-rgb-cycle-720.mp4     # H.264, ~2.9MB, mobile fallback
  rog-astral-5080-rgb-cycle-1080.webm   # VP9, ~4.9MB, modern browsers
  rog-astral-5080-rgb-cycle-poster.jpg  # 1080p poster frame
  rog-astral-5080-rgb-cycle-poster.webp # poster, modern
```

## Image inventory & suggested captions

| Slug | Source | Suggested caption | Best use |
|---|---|---|---|
| `rog-astral-5080-angled-fans-rgb` | IMG_1689 | The ROG Astral RTX 5080 OC installed in my Hyte Y70, three Axial-tech fans visible with the RGB top bar lit blue-to-purple. | Hero / lead |
| `rog-astral-5080-angled-fans-pink-rgb` | IMG_1690 | RGB cycle mid-magenta — the Astral's lighting transitions smoothly through the full spectrum. | Body, RGB section |
| `rog-astral-5080-front-three-quarter` | IMG_1691 | Three-quarter view showing the cooler thickness and ROG-branded collector card below. | Cooler design section |
| `rog-astral-5080-front-angled` | IMG_1692 | Front-angled showing the card's full length relative to the case width. | Build-fit section |
| `rog-astral-5080-front-on-fans` | IMG_1693 | Straight-on view of all three Axial-tech fans and the rotation dial at the card's end. | Hero alternative / fan design |
| `rog-astral-5080-side-profile` | IMG_1694 | Side profile — visible 3.5-slot thickness and the dual 8-pin power pass-through. | Specs / dimensions |
| `rog-astral-5080-installed-case` | IMG_1695 | Full case shot with the 5080 installed, NZXT Kraken 360 LCD reading CPU 51°C / GPU 29°C at idle. | Final build / system shot |
| `rog-astral-5080-rgb-strip-lit` | IMG_1696 | The top RGB bar at full brightness, individual segments addressable through Armoury Crate. | RGB / aesthetics |
| `rog-astral-5080-top-geforce-rtx-branding` | IMG_1697 | Top-down view showing the illuminated GeForce RTX text running along the card's top edge. | Branding detail |

## Video

| File | Notes |
|---|---|
| `rog-astral-5080-rgb-cycle-1080.mp4` | 17-second silent loop of the RGB color cycle in operation. Use with `<video autoplay muted loop playsinline>` for ambient embed. |
| Poster | Auto-generated at 2s mark, fans visibly spinning + RGB strip mid-cycle. |

## Hugo embed snippets

### Single image with srcset (drop into article body):

```html
<figure class="post-figure">
  <picture>
    <source
      type="image/webp"
      srcset="/images/gpu-reviews/rog-astral-rtx-5080/rog-astral-5080-front-on-fans-400.webp 400w,
              /images/gpu-reviews/rog-astral-rtx-5080/rog-astral-5080-front-on-fans-800.webp 800w,
              /images/gpu-reviews/rog-astral-rtx-5080/rog-astral-5080-front-on-fans-1600.webp 1600w"
      sizes="(max-width: 800px) 100vw, 1600px">
    <img
      src="/images/gpu-reviews/rog-astral-rtx-5080/rog-astral-5080-front-on-fans-1600.jpg"
      srcset="/images/gpu-reviews/rog-astral-rtx-5080/rog-astral-5080-front-on-fans-800.jpg 800w,
              /images/gpu-reviews/rog-astral-rtx-5080/rog-astral-5080-front-on-fans-1600.jpg 1600w"
      sizes="(max-width: 800px) 100vw, 1600px"
      width="1600" height="900"
      alt="ASUS ROG Astral RTX 5080 OC installed in operator's Hyte Y70 case, three Axial-tech fans facing the viewer"
      loading="lazy" decoding="async">
  </picture>
  <figcaption>Straight-on view of all three Axial-tech fans and the rotation dial at the card's end. Operator's primary rig, St. Louis County, MO.</figcaption>
</figure>
```

### Hero image (eager-load, top of article):

```html
<figure class="post-hero">
  <picture>
    <source type="image/webp"
      srcset="/images/gpu-reviews/rog-astral-rtx-5080/rog-astral-5080-angled-fans-rgb-800.webp 800w,
              /images/gpu-reviews/rog-astral-rtx-5080/rog-astral-5080-angled-fans-rgb-1600.webp 1600w"
      sizes="100vw">
    <img
      src="/images/gpu-reviews/rog-astral-rtx-5080/rog-astral-5080-angled-fans-rgb-1600.jpg"
      width="1600" height="900"
      alt="ASUS ROG Astral RTX 5080 OC angled view with RGB strip lit blue-purple"
      fetchpriority="high" decoding="async">
  </picture>
  <figcaption>The ROG Astral RTX 5080 OC installed in my Hyte Y70 — first-party photo, June 2026.</figcaption>
</figure>
```

### Ambient video embed:

```html
<figure class="post-video">
  <video
    autoplay muted loop playsinline
    poster="/videos/gpu-reviews/rog-astral-rtx-5080/rog-astral-5080-rgb-cycle-poster.jpg"
    width="1920" height="1080">
    <source src="/videos/gpu-reviews/rog-astral-rtx-5080/rog-astral-5080-rgb-cycle-1080.webm" type="video/webm">
    <source src="/videos/gpu-reviews/rog-astral-rtx-5080/rog-astral-5080-rgb-cycle-1080.mp4" type="video/mp4">
    <source src="/videos/gpu-reviews/rog-astral-rtx-5080/rog-astral-5080-rgb-cycle-720.mp4" type="video/mp4">
  </video>
  <figcaption>RGB cycle in operation — 17-second silent loop. Operator's primary rig.</figcaption>
</figure>
```

## Provenance & E-E-A-T notes (for AdSense reviewer audit trail)

- All photos and video captured 2026-06-13 by the operator on his own ROG Astral RTX 5080 OC card
- Source files retained in operator's photo library
- EXIF/GPS stripped before publication per `PROJECT_POLICY.md` §privacy
- Image filenames use the canonical review slug `rog-astral-rtx-5080`
- This manifest may be referenced from the review article's "Methods & sources" section

## Notes for CC

When you rebuild the ROG Astral 5080 review page during the redesign, swap the existing zero-image article body for the snippets above. Recommended placement:

- **Hero:** `rog-astral-5080-angled-fans-rgb` (the blue-RGB angled shot — strongest opening visual)
- **Build/install section:** `rog-astral-5080-installed-case`
- **Cooler design:** `rog-astral-5080-front-on-fans` + `rog-astral-5080-side-profile`
- **RGB/aesthetics:** `rog-astral-5080-rgb-strip-lit` + the video
- **Closing:** `rog-astral-5080-top-geforce-rtx-branding`

Don't dump all 9 into the page; pick 4-5 strongest. The video should appear once in the RGB or aesthetics section.

# Image slots

Drop files with these exact names into this folder and the site will pick
them up automatically — no HTML/CSS changes needed.

| File | Used for |
|---|---|
| `clinic-hero.jpg` | Hero section, right-side photo |
| `clinic-interior.jpg` | About section, clinic interior photo |
| `vet-ayse-demir.jpg` | Vet card — Dr. Ayşe Demir |
| `vet-can-ozkan.jpg` | Vet card — Dr. Can Özkan |
| `vet-elif-gunes.jpg` | Vet card — Dr. Elif Güneş |

Until a file exists, each slot shows an elegant CSS placeholder (a paw-print
icon for the two clinic photos, initials for each vet) instead of a broken
image — see `.photo-frame` / `.photo-fallback` in `css/styles.css`.
Recommended aspect ratios: 4:5 for the hero photo, 4:3 for the interior
photo, 1:1 for vet photos, matching what's already set in the CSS.

If you're sourcing real photos, resize/compress them first rather than
dropping in raw camera/stock exports — see the note in the Dentflow demo
site's equivalent `assets/img/README.md` for the exact `convert` command
used there (1200px wide for the two clinic photos, 900px for people
photos, JPEG quality 80).

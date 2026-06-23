# nutday2026
Birthday repo for our beloved Nat 

---
 
## Folder Structure
 
```
your-repo/
├── index.html          ← the app, already pushed
├── collage.jpg         ← upload this at the END of the day
└── photos/
    ├── 01.jpg          ← upload these throughout the day
    ├── 02.jpg
    ├── 03.jpg
    └── ... up to 20.jpg
```
 
### Naming rules
 
| File | Where | When to upload |
|------|-------|----------------|
| `index.html` | Root | Already done |
| `collage.jpg` | Root | End of day — appears on the birthday end page only |
| `photos/01.jpg` … `photos/20.jpg` | `/photos/` folder | Throughout the day |
 
- **Day photos** must be named with two digits, zero-padded: `01.jpg`, `02.jpg`, `03.jpg` … `20.jpg`. They appear in the gallery in this order, so name them in the sequence you want them displayed.
- **Collage** must be named exactly `collage.jpg` at the root level (same folder as `index.html`). If the file is not there yet, that section is simply hidden — no errors.
---
 
## Enabling GitHub Pages
 
1. Go to your repo → **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: `main` → Folder: `/ (root)`
4. Click **Save**
Your app will be live at:
```
https://yourusername.github.io/your-repo-name/
```
 
> It may take 1–2 minutes to go live after the first push.
 
---
 
## Uploading Photos During the Day
 
You can upload photos directly from GitHub's web UI without needing a computer:
 
1. Go to your repo on GitHub
2. Click into the `photos/` folder
3. Click **Add file → Upload files**
4. Drag in your photo, name it `05.jpg` (or whatever the next number is)
5. Click **Commit changes**
The gallery updates live as soon as the file is pushed — no rebuild needed.
 
---
 
## Uploading the Collage at End of Day
 
1. Go to your repo on GitHub
2. Click **Add file → Upload files** (from the root, not the photos folder)
3. Upload your collage image and name it exactly `collage.jpg`
4. Click **Commit changes**
Refresh the app and the collage will appear on the birthday end page.
 
---
 
## App Features
 
- **5 puzzles** — Nokia T9 decode, word search, Caesar cipher, Korean phonetics trap, K-pop first-letter cipher
- **1 bonus round** — Pokémon Pokédex puzzle
- **Progressive hints** — up to 2 hints per puzzle, revealed one at a time
- **Home button** (🏠) — resets progress back to Puzzle 1
- **Skip to End** (⏭) — jumps to the birthday end page
- **localStorage caching** — refreshing the page stays on the current puzzle
- **End page** — birthday messages, collage photo, photo gallery, full journey recap
- **Photo gallery** — 2-column scrollable grid of all day photos
---
 
## Generating the Birthday Collage
 
Give the following prompt to Claude or Gemini, with all the day's photos attached:
 
---
 
> I need you to describe in precise detail how to recreate the following collage aesthetic in Canva (or CapCut), using the photos I'm attaching. I want step-by-step instructions tailored to these exact photos.
>
> **Reference aesthetic:**
> - Canvas size: 9:16 portrait (phone wallpaper ratio), white or very light cream background
> - 7–9 photos arranged in a scattered, overlapping layout — no grid, no alignment
> - 2–3 photos are treated as "cut-outs": the people are cut out from their background (use Canva's Background Remover or CapCut's Smart Cutout), so only the subject floats on the canvas
> - 1 photo has a Polaroid-style frame: white border, thicker at the bottom, slight drop shadow
> - All photos are rotated between −12° and +12°, each at a different angle — nothing is straight
> - Photos overlap each other, with some layered on top of others
> - The largest photo is centred and takes up roughly 40% of the canvas height
> - Smaller photos surround it, placed near the corners and edges
>
> **Text overlay:**
> - "Happy Birthday Nat!" in a flowing white brush/script font (use Playlist Script, Great Vibes, or Dancing Script in Canva) — large, placed in the upper-centre area, overlapping the photos
> - Font size should feel like it covers roughly 30% of the canvas width
> - Add a very subtle dark shadow or slight outline so the text reads clearly over the photos
>
> **Decorative elements:**
> - 6–8 white four-pointed sparkle stars (✦) scattered around the canvas — different sizes, some near photo corners, some floating in open space. In Canva, search "sparkle" or "4-point star" in Elements. In CapCut, use Stickers → Sparkle.
> - Optionally: a thin white irregular dashed border running loosely around 2–3 of the cut-out photos, as if torn from a page
>
> **Colour treatment:**
> - Slightly warm/golden colour grade overall — in Canva, apply a warm photo filter (e.g. "Fade" or "Glow") at 30–40% intensity to all rectangular photos
> - Cut-outs keep their natural colour
>
> **What I need from you:** Look at the photos I've attached and tell me — which photo should be the large central one, which 2–3 should be cut-outs, which should get the Polaroid frame, and where to position the rest. Then give me the step-by-step Canva instructions to build it.
 
---
 
Attach all the day's photos to that message. The AI will look at them and tell you which photo goes where, then walk you through building it in Canva or CapCut step by step.
# How to Fix Missing Photos on Your Site

The site expects all images to live in a folder named **`photos`** in the **same folder as `index.html`**.

---

## Step 1: Open your project folder

In Finder, go to:

**Desktop → feroleto-site**

You should see `index.html` there. If you also see a folder called `photos`, open it and go to Step 2. If you don’t see `photos`, go to Step 1b.

### Step 1b: Create the `photos` folder (if it doesn’t exist)

1. In the **feroleto-site** folder (same place as `index.html`), right‑click (or Control‑click).
2. Choose **New Folder**.
3. Name the folder exactly: **photos** (all lowercase, no spaces).

---

## Step 2: Put the right image files inside `photos`

The site looks for these **exact** file names inside the `photos` folder. Spelling, capitalization, and extension (`.jpg`) must match.

| File name | Where it’s used |
|-----------|------------------|
| `hero-harvest-basket.jpg` | Hero (full‑width top) — you said this one works |
| `lettuce-raised-bed.jpg` | Full‑width section after About |
| `zinnia-field.jpg` | Full‑width section after Garden Co. |
| `tomato-harvest.jpg` | Gallery, 1st image |
| `dahlia-cafe-au-lait.jpg` | Gallery, 2nd image |
| `poppies.jpg` | Gallery, 3rd image |
| `dahlia-pink-yellow.jpg` | Gallery, 4th image |
| `dahlia-sunset.jpg` | Gallery, 5th image |
| `dahlia-cream.jpg` | Gallery, 6th image |

- Copy or move your image files into the **photos** folder.
- If a file has a different name (e.g. `Dahlia Cafe au Lait.jpg`), **rename it** to match the table (e.g. `dahlia-cafe-au-lait.jpg`). Use lowercase and hyphens as shown.
- Make sure the extension is **.jpg** (or **.jpeg** — see Step 3).

---

## Step 3: Check file names and extensions

1. Open the **photos** folder.
2. Turn on “Show filename extensions” if you don’t see them: **Finder → Settings (or Preferences) → Advanced → check “Show all filename extensions”.**
3. For each file in the table above, confirm:
   - The name matches **exactly** (including hyphens and no spaces).
   - The extension is **.jpg** (or **.jpeg** — if you use `.jpeg`, the site won’t find it unless we change the code; sticking to **.jpg** is easiest).

---

## Step 4: Reload the site

1. Save any changes and close the **photos** folder.
2. Open **index.html** in your browser (double‑click it, or drag it into Chrome/Safari/Firefox).
3. Do a **hard refresh** so the browser doesn’t use old cached content:
   - **Mac:** `Cmd + Shift + R` (Chrome/Safari/Firefox).
   - Or close the tab and open **index.html** again.

You should now see the two full‑width photo sections and the six gallery images, as long as the files in **photos** match the names in the table.

---

## Quick checklist

- [ ] Folder name is **photos** (lowercase), next to **index.html**.
- [ ] All 9 files from the table are inside **photos**.
- [ ] File names match exactly (e.g. `lettuce-raised-bed.jpg`, not `Lettuce Raised Bed.JPG`).
- [ ] Extensions are **.jpg**.
- [ ] You did a hard refresh (or reopened the page) after adding/renaming files.

---

## If you’re still missing some images

- **Only have a few photos?** Put in the ones you have using the exact names from the table. The hero, lettuce, and zinnia sections use one image each; the gallery uses the six listed. Missing files will show as broken images or empty areas until you add them.
- **Using a different format (e.g. .png)?** The site is written for **.jpg** only. Either export/save your images as **.jpg** and use the names above, or we can change the code to point to **.png** for specific files.
- **Deploying to Netlify (or similar)?** Upload the **photos** folder together with **index.html** in the same structure (so the live site has `photos/hero-harvest-basket.jpg`, etc.). The same names and folder structure apply online.

Once your **photos** folder matches this setup, the hero, two full‑width breaks, and gallery should all show correctly.

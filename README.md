# subtext-data

GitHub Pages site that serves data files (CSV) for the Subtext Shopify store. The storefront fetches these files at runtime.

**Live URL:** `https://colecharb.github.io/subtext-data/Grind_Map_Data.csv`

## How to update the CSV

### Option A: GitHub UI (easiest)
1. Go to the `/docs` folder in this repo on GitHub
2. Click **Add file → Upload files**
3. Drag and drop your updated `Grind_Map_Data.csv`
4. Commit the change

### Option B: Git
```bash
cp /path/to/Grind_Map_Data.csv docs/Grind_Map_Data.csv
git add docs/Grind_Map_Data.csv
git commit -m "Update grind map data"
git push
```

## Verify changes are live

After pushing, GitHub Pages deploys automatically (usually within a minute). Visit:

`https://colecharb.github.io/subtext-data/Grind_Map_Data.csv`

If the file downloads with your latest data, you're good.

> **Note:** The Shopify component fetches this file with a cache-buster query param (`?t=${Date.now()}`), so visitors will always get the latest version without browser caching issues.

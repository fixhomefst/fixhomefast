# 🔧 FixHomeFast — Premium SEO Edition v4

**Clean, premium, SEO-optimized DIY home solutions blog.**

> Single HTML file. No build step. Deploy in 30 seconds.

---

## ✨ What's New in v4

| Feature | Details |
|---|---|
| 🎨 Clean Layout | Champagne gold on deep charcoal — no messy background clutter |
| 🖼️ SVG Thumbnails | Unique, hand-crafted SVG art per category — no external images needed |
| 🔍 Full SEO | Meta title, description, focus keyword, schema markup per article |
| 📍 Geo Targeting | US geo meta tags, English-US language targeting |
| 🔗 Internal Linking | Every article links to 3–4 related articles with anchor text |
| 📊 Schema Markup | Website + Blog + HowTo schema on every article page |
| 🗝️ Long-tail Keywords | Every article targets a specific high-volume long-tail keyword |
| 📰 20 Full Articles | Complete HTML bodies with H2/H3 structure, tips, warnings, tables |
| 🗂️ Category Filter | Filter + paginate all 20+ articles by category |
| ⚙️ Admin Dashboard | Login (admin / fixhome2025) — write, edit, delete articles |
| 💾 localStorage | All admin changes persist across sessions |
| 📱 Mobile Responsive | Works on all screen sizes |
| 💰 AdSense Ready | Clean structure, original content, no keyword stuffing |

---

## 🗂️ File Structure

```
fixhomefast/
├── index.html     ← Complete website
├── vercel.json    ← Security headers + routing
└── README.md      ← This file
```

---

## 🚀 Deploy

### Vercel (Recommended)
```bash
git init
git add .
git commit -m "FixHomeFast v4 launch"
git branch -M main
git remote add origin https://github.com/YOURNAME/fixhomefast.git
git push -u origin main
```
Then: vercel.com → Import → Deploy ✅

### GitHub Pages
Repo → Settings → Pages → Source: `main` branch `/root`

### Local
```bash
open index.html
# or
npx serve .
```

---

## ⚙️ Admin Panel

Click **Admin** in the nav bar.

| Field | Value |
|---|---|
| Username | `admin` |
| Password | `fixhome2025` |

**Admin can:**
- 📊 View article statistics
- ✏️ Write new articles with full HTML body
- 🖊️ Edit any existing article
- 🗑️ Delete articles
- 🔑 Set SEO focus keyword per article
- 📝 Set meta title + meta description per article
- 💾 All changes saved to browser localStorage

**Change the password** — find in `index.html`:
```javascript
const AU='admin', AP='fixhome2025';
```

---

## 📝 SEO Structure

Each article includes:

```javascript
{
  id:       'slug-for-url',
  title:    'Full Article Title',
  kw:       'focus keyword phrase',        // Long-tail keyword
  meta:     'SEO Page Title | FixHomeFast', // 50–60 chars
  metaDesc: 'Meta description...',          // 150–160 chars
  body:     `<h2>...</h2><p>...</p>`        // Full HTML with H2/H3
}
```

**Schema markup** injected dynamically on article open:
- `WebSite` schema on homepage
- `Blog` schema on homepage
- `HowTo` schema on every article page

**Internal linking** — every article body contains:
```html
<div class="ilink-box">
  <strong>🔗 Related Guides</strong>
  <a onclick="openArticle('related-id')">→ Related Article Title</a>
</div>
```

---

## 🎨 Customise Colors

```css
:root {
  --gold:    #c9a84c;   /* Main accent */
  --gold-l:  #e8c46a;   /* Light accent */
  --gold-d:  #9e7f32;   /* Dark accent */
  --bg:      #0e0e0e;   /* Background */
  --t1:      #f2edd8;   /* Primary text */
  --t2:      #a89f8c;   /* Secondary text */
}
```

---

## 💰 AdSense Setup

Find the comment `<!-- AdSense -->` in the HTML and paste your `<ins>` tag.

**AdSense compliance checklist:**
- ✅ 20 original, high-quality articles
- ✅ Clear navigation and category structure
- ✅ Privacy Policy + Disclaimer links in footer
- ✅ No keyword stuffing
- ✅ Mobile responsive
- ✅ Fast loading (no heavy 3D, CDN fonts only)
- ✅ Unique SVG thumbnails (no copyright issues)

---

## 🔍 SEO Keywords Targeted

| Article | Focus Keyword |
|---|---|
| Oil Stains | how to remove oil stains from clothes |
| Cockroaches | how to get rid of cockroaches naturally |
| Dripping Faucet | how to fix a dripping faucet yourself |
| Bathroom Cleaning | how to deep clean bathroom fast |
| Gas Burner | gas burner not lighting fix |
| Squeaky Floor | how to fix squeaky floorboard without lifting |
| Red Wine | how to remove red wine stains from carpet |
| Cool Room | how to keep room cool without air conditioning |
| Kitchen Ants | how to get rid of kitchen ants naturally |
| Shower Drain | how to unclog shower drain without tools |
| Grout Mold | how to remove mold from bathroom grout |
| Fridge Fix | refrigerator not cooling fix |
| Window Fix | how to fix window that wont stay open |
| Blood Stains | how to remove blood stains from sheets |
| Mice | how to get rid of mice yourself |
| Oven Clean | how to clean oven without chemicals |
| Coffee Stain | how to remove coffee stains from clothes |
| Shower Pressure | how to fix low shower pressure |
| Kitchen Sink | how to unclog kitchen sink without chemicals |
| Noise Walls | how to reduce noise through thin walls |

---

© 2025 FixHomeFast. Built for homeowners who fix things themselves.

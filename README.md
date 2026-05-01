# 🔧 FixHomeFast — Ultra Premium Edition

**Live DIY home solutions blog. Fast. Beautiful. AdSense-ready.**

> Deploy in 30 seconds. No build step. No framework. Just upload and go.

---

## ✨ What's Inside

| Feature | Details |
|---|---|
| 🎬 Welcome Screen | Cinematic animated intro on every load |
| ✦ Particle Hero | Live animated canvas with connected dots |
| 🖱️ Custom Cursor | Magnetic cursor with hover morphing effect |
| 🎞️ Ticker Tape | Scrolling category strip in fire orange |
| 🗂️ Bento Grid | Editorial magazine-style post layout |
| 🖼️ Real Images | Unsplash photos on all article cards |
| 📐 3D Tilt Cards | Mouse-tracked perspective tilt on hover |
| 🔤 Bebas + Fraunces | Premium editorial font pairing |
| 📱 Mobile Responsive | Full-screen slide-in mobile menu |
| 📬 Newsletter Section | Dark section with animated blob background |
| 🔍 SEO Ready | Meta tags, schema markup, canonical URLs |
| 💰 AdSense Ready | Clean structure, original content, clear nav |

---

## 🗂️ File Structure

```
fixhomefast/
├── index.html     ← Entire website (HTML + CSS + JS, single file)
├── vercel.json    ← Vercel headers + routing config
└── README.md      ← This file
```

---

## 🚀 Deploy to Vercel (30 seconds)

### Option A — Drag & Drop
1. Go to [vercel.com](https://vercel.com) → New Project
2. Drag the folder in
3. Click Deploy ✅

### Option B — Via GitHub
```bash
# In the project folder:
git init
git add .
git commit -m "launch FixHomeFast v2"
git branch -M main
git remote add origin https://github.com/YOURNAME/fixhomefast.git
git push -u origin main
```
Then: Vercel → Import → select repo → Deploy.

### Option C — GitHub Pages
1. Repo → Settings → Pages
2. Source: `main` branch, `/ (root)`
3. Save → live at `https://yourusername.github.io/fixhomefast`

---

## 📝 Adding New Articles

**Step 1** — Add to `POSTS` array (line ~310 in index.html):
```javascript
{
  id: 'your-slug',
  cat: 'Home Cleaning',         // must match a category
  icon: '🧹',                   // fallback if image fails
  title: 'Your Article Title',
  time: '5 min',
  img: 'https://images.unsplash.com/photo-XXXXXXX?w=600&h=340&fit=crop',
  exc: 'Short excerpt shown on featured cards.'
},
```

**Step 2** — Add full article to `ARTICLES` object (line ~390):
```javascript
'your-slug': {
  meta: {
    title: 'Your Article Title',
    cat: 'Home Cleaning',
    date: 'June 2025',
    time: '5 min',
    img: 'https://images.unsplash.com/photo-XXXXXXX?w=1200&h=500&fit=crop'
  },
  body: `
    <p>Your intro paragraph here.</p>
    <h2>Section Heading</h2>
    <p>Content here...</p>
    <div class="tip-box"><strong>💡 Tip</strong><p>Tip text.</p></div>
    <div class="warn-box"><strong>⚠️ Warning</strong><p>Warning text.</p></div>
  `
},
```

---

## 💰 AdSense Setup

Find this comment in index.html:
```html
<!-- AdSense: paste your <ins> tag here -->
```
Replace with your AdSense code block.

---

## 🎨 Changing Colors

Edit CSS variables at the top of the `<style>` block:
```css
:root {
  --fire: #e85d04;    /* main accent — change to any color */
  --ember: #f48c06;   /* secondary accent */
  --gold: #ffd60a;    /* highlight color */
  --ink: #09090b;     /* dark background */
  --paper: #fafaf9;   /* page background */
}
```

---

## 📄 License

Free to use for personal and commercial projects.

---

Built with 🔥 for homeowners who fix things themselves.

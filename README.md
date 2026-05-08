# SF Tapas — Website

Authentic Spanish Tapas & Paella Catering in San Francisco.

Live site: [https://YOUR-USERNAME.github.io/sf-tapas](https://YOUR-USERNAME.github.io/sf-tapas)

---

## 🚀 How to Deploy on GitHub Pages

### Option A — Upload via GitHub.com (no coding required)

1. Go to [github.com](https://github.com) and sign in (or create a free account)
2. Click **"New repository"** (the green button)
3. Name it `sf-tapas` — make sure it is set to **Public**
4. Click **"Create repository"**
5. On the next screen, click **"uploading an existing file"**
6. Drag and drop `index.html` into the upload area
7. Click **"Commit changes"**
8. Go to **Settings → Pages** (left sidebar)
9. Under **"Branch"**, select `main` and click **Save**
10. Wait ~60 seconds, then visit: `https://YOUR-USERNAME.github.io/sf-tapas`

---

### Option B — Using Git (command line)

```bash
git init
git add index.html
git commit -m "Initial commit — SF Tapas website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/sf-tapas.git
git push -u origin main
```

Then enable GitHub Pages in **Settings → Pages → Branch: main → Save**.

---

## 📁 File Structure

```
sf-tapas/
├── index.html      ← The complete website (single file, no dependencies)
└── README.md       ← This file
```

The site is fully self-contained in `index.html`:
- All CSS is embedded in `<style>` tags
- All JavaScript is inline
- Google Fonts loads via CDN (requires internet connection)
- No frameworks, no build tools, no npm

---

## 🖼 Adding Real Images

All images are currently placeholders. To replace them:

1. Create an `images/` folder in your repository
2. Upload your photos there
3. Open `index.html` and find the placeholder `<div>` elements
4. Replace each placeholder `<div>` with an `<img>` tag:

```html
<!-- Replace this -->
<div class="hero-img-placeholder"></div>

<!-- With this -->
<img src="images/hero-paella.jpg" alt="Live paella cooking at a San Francisco event" 
     style="position:absolute;inset:0;width:100%;height:100%;object-fit:cover;">
```

**Recommended image specs:**
| Section | File name suggestion | Size |
|---|---|---|
| Hero background | `hero-paella.jpg` | 1920×1080px |
| Gallery image 1 | `gallery-croquetas.jpg` | 900×600px |
| Gallery image 2 | `gallery-shrimp.jpg` | 900×600px |
| Gallery image 3 | `gallery-paella-cook.jpg` | 900×600px |
| Gallery image 4 | `gallery-paella-wide.jpg` | 900×600px |
| Gallery image 5 | `gallery-event.jpg` | 900×600px |
| Gallery image 6 | `gallery-tapas-spread.jpg` | 900×600px |
| Signature section | `signature-cooking.jpg` | 800×1040px |
| Our Story section | `story-kitchen.jpg` | 800×1080px |

---

## ✏️ Updating Content

All text is in plain HTML. Open `index.html` in any text editor (VS Code, Notepad, TextEdit) and search for the text you want to change.

**Key things to update before going live:**
- [ ] Replace `info@sftapas.com` with your real email address
- [ ] Replace `+14155550000` with your real phone number
- [ ] Replace `[Client Name]` placeholders in testimonials with real names
- [ ] Replace `YOUR-USERNAME` in this README with your GitHub username
- [ ] Add real photos (see image guide above)

---

## 🔗 Custom Domain (optional)

To use `www.sftapas.com` instead of the github.io URL:

1. Create a file named `CNAME` in the repository root
2. Add your domain as the only line: `www.sftapas.com`
3. Go to your domain registrar and add a CNAME DNS record pointing to `YOUR-USERNAME.github.io`
4. In GitHub → Settings → Pages → Custom domain, enter `www.sftapas.com`
5. Check **"Enforce HTTPS"**

---

## 📋 Migration to Odoo

This file is a design reference and working website. When you're ready to migrate to Odoo Bistro, refer to the section-by-section Odoo migration guide for mapping each section to its native Bistro snippet.

---

*Built for SF Tapas — San Francisco's Spanish culinary experience.*

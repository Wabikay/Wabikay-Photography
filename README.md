# Wabikay Photography Website
**Capturing Stories. Preserving Legacy.**

Live site for Wabikay Photography — Lagos, Nigeria.

---

## 📁 Project Files

```
wabikay-photography/
├── index.html        ← The entire website (edit this)
├── netlify.toml      ← Netlify settings (don't touch)
├── .gitignore        ← Tells Git what to ignore (don't touch)
└── README.md         ← This guide
```

---

## 🚀 STEP-BY-STEP DEPLOYMENT GUIDE

### PART 1 — Set Up GitHub (one time only)

1. Go to **github.com** and create a free account
2. Click the **+** icon (top right) → **New repository**
3. Name it: `wabikay-photography`
4. Set to **Public**
5. Click **Create repository**
6. Click **uploading an existing file** (shown on the next screen)
7. Drag ALL your files into the upload area:
   - index.html
   - netlify.toml
   - .gitignore
   - README.md
8. Scroll down → click **Commit changes**

✅ Your files are now on GitHub.

---

### PART 2 — Deploy on Netlify (one time only)

1. Go to **netlify.com** → Sign up free (use your GitHub account to sign in)
2. Click **Add new site** → **Import an existing project**
3. Click **GitHub**
4. Select your `wabikay-photography` repository
5. Leave all settings as default
6. Click **Deploy site**
7. Wait ~30 seconds → your site is LIVE!

You'll get a URL like: `https://wabikay-photography.netlify.app`

---

### PART 3 — Custom Domain (optional, ~$10/year)

1. Buy a domain at **namecheap.com** (e.g. `wabikayphotography.com`)
2. In Netlify dashboard → **Domain settings** → **Add custom domain**
3. Type your domain name → follow the instructions
4. Netlify handles HTTPS/SSL automatically for free

---

## ✏️ HOW TO UPDATE YOUR SITE

Every time you want to make a change:

1. Open `index.html` on your computer in any text editor
   - Windows: Notepad, Notepad++, or VS Code
   - Mac: TextEdit (plain text mode) or VS Code
2. Make your changes and save the file
3. Go to your GitHub repository
4. Click on `index.html`
5. Click the **pencil icon** (Edit this file)
6. Paste your updated content
7. Click **Commit changes**
8. Netlify automatically detects the change and redeploys
9. Your site updates live in ~30 seconds ✅

---

## 🖼️ HOW TO ADD YOUR REAL PHOTOS

### Option A — Use direct image URLs (easiest)
Host images on Google Photos, Cloudinary, or ImgBB, then replace
the placeholder divs in index.html like this:

**Find this (placeholder):**
```html
<div class="gallery-item" onclick="openLightbox(this)">
  <div class="gallery-placeholder gp-1"></div>
  ...
</div>
```

**Replace with:**
```html
<div class="gallery-item" onclick="openLightbox(this)">
  <img src="YOUR_IMAGE_URL_HERE" alt="Wedding photography Lagos" 
       style="width:100%;height:100%;object-fit:cover;" loading="lazy" />
  ...
</div>
```

### Option B — Upload images to GitHub
1. In your GitHub repo, create a folder called `images`
2. Upload your photos there
3. Use the path: `images/your-photo-name.jpg`

---

## 🔗 HOW TO ADD GOOGLE PHOTOS ALBUMS

1. Open Google Photos on the web
2. Open an album → click Share → **Get link**
3. In index.html, find the portfolio notice sections
4. Replace `[ADD GOOGLE PHOTOS LINK]` with your album link

---

## 📬 HOW TO ACTIVATE THE BOOKING FORM (send real emails)

1. Go to **formspree.io** → sign up free
2. Create a new form → copy your form endpoint (looks like `https://formspree.io/f/xxxxxxxx`)
3. In index.html, find the `submitBookingForm()` function
4. Replace the comment with:
```javascript
fetch('https://formspree.io/f/YOUR_CODE_HERE', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify({ name, email, phone, eventType })
});
```

---

## 📍 HOW TO ADD GOOGLE MAPS

1. Go to **maps.google.com**
2. Search your location in Lagos
3. Click Share → **Embed a map** → Copy the iframe code
4. In index.html, find `<div class="map-placeholder">` and replace it with the iframe

---

## 📞 CONTACT

- Phone: +234 814 913 9188
- Email: wabikay@gmail.com
- Instagram: @lightandnarrative
- WhatsApp: https://wa.me/2348149139188

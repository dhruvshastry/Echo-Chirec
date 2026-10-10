# The Echo — Modern Website (Prototype)

CHIREC CBSE’s student-run newspaper redesign.

## Pages
- `index.html` — Home
- `issues.html` — All issues archive
- `issue-november-2025.html` / `issue-january-2025.html` — Full issue viewers
- `article-india-vs-maldives.html` — Editor’s Pick article
- `photojournalism.html` — Photojournalism gallery
- `masthead.html` — Team / Core Team

## How to open locally
1. Unzip the folder
2. Double-click `index.html`

---

## How to get a sendable link (share with the team)

### Option A — GitHub Pages (free, recommended)

1. Create a free account at [github.com](https://github.com) if you don’t have one
2. Click **New repository** → name it e.g. `the-echo` → make it **Public** → Create
3. Click **uploading an existing file** and drag **all files inside** the `echo-modern` folder (not the folder itself) into the upload area
4. Click **Commit changes**
5. Go to **Settings → Pages**
6. Under “Source”, choose **Deploy from a branch** → Branch: `main` → Folder: `/ (root)` → Save
7. Wait 1–2 minutes. Your live link will be:

   **`https://YOUR-USERNAME.github.io/the-echo/`**

   Share that URL with the team.

### Option B — Netlify Drop (fastest, no account required for a temporary link)

1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag the entire `echo-modern` folder onto the page
3. You’ll instantly get a public link like `https://random-name.netlify.app`
4. Share that link. (You can claim it with a free Netlify account to keep it permanently.)

### Option C — Local live server (only on the same Wi-Fi)

```bash
# If you have Python installed:
cd echo-modern
python -m http.server 8000
```

Then open `http://localhost:8000` on your computer.  
Others on the same Wi-Fi can use `http://YOUR-IP:8000` (find your IP with `ipconfig` / `ifconfig`).

---

## Replacing placeholder photos

In `photojournalism.html`, each card has a placeholder icon.  
To add real photos, replace the `.photo-card-img` content with:

```html
<img src="assets/your-photo.jpg" alt="Description" style="width:100%;height:100%;object-fit:cover;" />
```

Put the image files in the `assets/` folder.

## Custom domain later

Once on GitHub Pages or Netlify you can point `echochirec.in` (or a subdomain) to the new site when you’re ready to replace the old WordPress one.

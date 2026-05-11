# CNRL Open House 2026 — Website

Website for the **Chiari Neurobiomechanics Research Laboratory Open House**  
**August 8, 2026 · ISEC Building · Northeastern University**

---

## File Structure

```
CNRLpage/
├── index.html          ← Main single-page website
├── css/
│   └── style.css       ← All styles (Northeastern Red & Black theme)
├── images/
│   └── (add your images here — see below)
└── README.md           ← This file
```

---

## Filling In Your Content

Open `index.html` in any text editor and search for `<!-- TODO:` to find every
placeholder that needs your real content. Key areas:

| Section | What to fill in |
|---------|----------------|
| **About** | Edit the two `<p>` paragraphs describing the event |
| **Schedule** | Replace placeholder rows with rows from `Agenda_2026.docx` |
| **Speakers** | Replace each `speaker-card` with real name, title, bio, and photo |
| **Posters** | Replace placeholder `<li>` items from `list posters_presentations.docx` |
| **Location** | Confirm room number, update contact email |
| **Footer** | Update contact email |

### Adding Speaker Photos

1. Save each photo as a `.jpg` or `.png` into the `images/` folder  
   (e.g., `images/speaker_jane_doe.jpg`)
2. In each speaker card, replace the `<div class="speaker-img-placeholder">` block with:

```html
<img src="images/speaker_jane_doe.jpg" alt="Jane Doe" class="speaker-img" />
```

---

## Hosting on GitHub Pages

### Step 1 — Create a GitHub repository

1. Log in to GitHub as the **Neurobiomechanics** organization  
   (or a personal account — adjust the URL in Step 4 accordingly)
2. Click **New repository**
3. Name it `open-house-2026` (or any name you prefer)
4. Set visibility to **Public** (required for free GitHub Pages)
5. Do **not** initialize with a README (you already have one)
6. Click **Create repository**

### Step 2 — Push your files

In Terminal, from inside the `CNRLpage/` folder:

```bash
git init
git add .
git commit -m "Initial CNRL Open House 2026 website"
git branch -M main
git remote add origin https://github.com/Neurobiomechanics/open-house-2026.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages

1. In your repository on GitHub, go to **Settings → Pages**
2. Under **Source**, select **Deploy from a branch**
3. Choose branch: `main`, folder: `/ (root)`
4. Click **Save**

### Step 4 — Your live URL

After ~1–2 minutes your site will be live at:

```
https://neurobiomechanics.github.io/open-house-2026/
```

### Updating the site after changes

Every time you push changes to `main`, GitHub Pages will automatically redeploy:

```bash
git add .
git commit -m "Update schedule / add speaker bios"
git push
```

---

## Local Preview

You can open `index.html` directly in any browser — no server needed — to
preview your changes before pushing to GitHub.

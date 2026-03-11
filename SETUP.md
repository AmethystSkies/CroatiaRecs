# How to Publish This Guide on GitHub

## Quick Setup (5 minutes)

### Step 1: Create the Repository on GitHub

1. Go to [github.com/new](https://github.com/new)
2. Fill in:
   - **Repository name:** `croatia-travel-guide`
   - **Description:** `🇭🇷 A complete personal travel guide to Croatia — curated recommendations, Google Maps links, and the Bourdain Route`
   - **Public** (so others can see it)
   - **Do NOT** check "Add a README file" (we already have one)
3. Click **Create repository**

### Step 2: Upload the Files

**Option A: Upload via GitHub Web UI (Easiest)**

1. On your new empty repo page, click **"uploading an existing file"** link
2. Drag and drop ALL of these files/folders into the upload area:
   - `README.md`
   - `LICENSE`
   - `images/` folder (with all 7 crest PNG files inside)
3. In the commit message, type: `Initial commit: Croatia Travel Guide by Niko Zivanovich`
4. Click **Commit changes**

**Option B: Upload via Git Command Line**

Open your terminal and run these commands:

```bash
# Navigate to the folder containing the repo files
cd path/to/croatia-travel-guide

# Initialize git
git init

# Set your author info
git config user.name "Niko Zivanovich"
git config user.email "your-email@example.com"

# Add all files
git add .

# Commit
git commit -m "Initial commit: Croatia Travel Guide by Niko Zivanovich"

# Set main branch
git branch -M main

# Add your GitHub repo as remote (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/croatia-travel-guide.git

# Push
git push -u origin main
```

### Step 3: Verify

1. Go to `https://github.com/YOUR_USERNAME/croatia-travel-guide`
2. You should see the README rendering with the Croatian coat of arms, table of contents, and all sections
3. All images should display inline
4. All Google Maps links should be clickable

### Step 4 (Optional): Add a GitHub Pages Site

If you want a standalone website version:

1. Go to your repo → **Settings** → **Pages**
2. Under "Source", select **Deploy from a branch**
3. Select **main** branch, **/ (root)** folder
4. Click **Save**
5. Your guide will be live at `https://YOUR_USERNAME.github.io/croatia-travel-guide/`

---

## Repository Structure

```
croatia-travel-guide/
├── README.md              # The full travel guide (renders on GitHub)
├── LICENSE                # MIT License
├── SETUP.md               # This file (setup instructions)
└── images/
    ├── crest_croatia.png          # Title: Croatian coat of arms
    ├── crest_zagreb.png           # Zagreb & Continental Croatia
    ├── crest_istria.png           # Istria Peninsula
    ├── crest_kvarner.png          # Kvarner Gulf
    ├── crest_dalmatia.png         # Northern Dalmatia
    ├── crest_dalmatia_central.png # Central Dalmatia
    └── crest_dubrovnik.png        # Southern Dalmatia (Dubrovnik)
```

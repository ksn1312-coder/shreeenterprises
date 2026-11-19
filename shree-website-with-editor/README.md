# Shree Enterprises: website and editor

A fast, mobile-friendly website with a **built-in editor**, so Shree's team can change text and photos without touching code.

| File | What it is |
|---|---|
| `index.html` | The website |
| `admin.html` | The editor (open it at `…/admin.html`) |
| `content/site.json` | All the text, lists, contacts and image paths. The editor writes this file for you. |
| `img/` | Photos. New uploads go into `img/uploads/`. |

---

## One-time setup (about 10 minutes)

**1. Put the site on GitHub Pages**
1. Open the repository (for example `github.com/ksn1312-wq/shreeenterprises`).
2. Click **Add file → Upload files** and drag in everything from this folder, **including the `content` and `img` folders**. Then click **Commit changes**.
3. Go to **Settings → Pages**, set **Source: Deploy from a branch** with branch **main** and folder **/ (root)**, then click **Save**.
4. After about a minute the site is live at `https://<owner>.github.io/<repo>/`.

**2. Create an access token for the editor**
1. On GitHub: **profile picture → Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**.
2. Name it `Shree website editor` and set an expiry (1 year works well).
3. Under **Repository access**, choose **Only select repositories** and pick the website repository.
4. Under **Permissions → Repository permissions → Contents**, choose **Read and write**.
5. Click **Generate token** and copy it. GitHub shows it only once.

**3. Connect the editor**
1. Open `https://<owner>.github.io/<repo>/admin.html`.
2. Click **⚙ Settings**. On GitHub Pages the owner and repository fill in automatically. Paste the token, then click **Test connection → Save**.
3. Do this once on each computer or phone you edit from. The token stays in that browser only.

---

## Everyday editing

1. Open **…/admin.html**.
2. Pick a section on the left: Header & Hero, Promo banners, Capabilities, Plant Models, Products, Clients, Contact and so on.
3. Change text, or click **⬆ Upload new** to replace a photo. Photos are resized and compressed automatically.
4. Use **+ Add**, **↑ ↓** and **✕** to add, reorder or remove models, products, clients, process steps and other items.
5. Check the **live preview** on the right. Switch between Desktop and Mobile.
6. Click **🚀 Publish**. The live site updates in about 1–2 minutes.

A green dot marks sections with unpublished changes. Unpublished work is kept in the browser, so you can close the tab and continue later.

**Photo tips**
- Hero background: a wide landscape photo, 1600 px or more across.
- Products: the item on a white background.
- Plant models: a 3:2 landscape photo.
- Use only photos and logos you have the right to use.

**Undo a change:** every Publish is saved in the repository history. On GitHub, open the repository's **Commits**, find the update and click **Revert**, or ask your web person to roll it back.

**No GitHub?** Click **⬇ Download** in the editor. It gives you a zip of the changed files (`content/site.json` plus any new photos). Upload them to the same folders on whatever host you use.

---

## Good to know
- The editor page is public, but nobody can change the site without the token.
- If a token leaks or someone leaves, delete it on GitHub (**Settings → Developer settings**) and create a new one.
- The website must be opened through a web address. Double-clicking `index.html` on your computer won't load the content.

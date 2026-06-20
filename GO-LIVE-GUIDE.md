# Tampa Bay Property Experts — Go-Live & Editing Guide

This is your real website. It keeps the custom design we built, **plus** a simple browser-based admin panel where you log in and edit text, swap photos, and publish blog posts — no code. Hosting is **free**.

Here's how it works in one sentence: your content lives in a code repository on GitHub, **Netlify** turns it into the live website automatically, and **Decap CMS** (the `/admin` panel) lets you edit that content from any browser.

---

## What's in this project

- `src/` — the website source (pages, blog posts, images, the editable data files). **This is the source of truth.**
- `src/admin/` — the editing panel (Decap CMS).
- `src/blog/` — blog posts (one Markdown file each). New posts you create in `/admin` land here automatically.
- `src/_data/site.json` & `src/_data/home.json` — your phone, email, address, and homepage hero text (editable in `/admin`).
- `styles.css` — the site's design/styling.
- `.eleventy.js`, `netlify.toml`, `package.json` — build settings (you don't need to touch these).

> The older standalone `.html` files in the top folder were the earlier static draft. They're no longer used by the live build and can be deleted whenever you like.

---

## Part 1 — Put it online (one-time, ~20 minutes)

You'll create two free accounts: **GitHub** (stores the files) and **Netlify** (hosts the live site). Don't worry — no coding.

### Step 1: Create a free GitHub account
Go to **github.com** and sign up.

### Step 2: Upload the project to a new repository
1. On GitHub, click **New repository**. Name it `tbpe-website`, keep it Private or Public, click **Create repository**.
2. On the new repo page, click **uploading an existing file**.
3. Drag in **everything** from this project folder (the `src` folder, `styles.css`, `.eleventy.js`, `netlify.toml`, `package.json`, `.gitignore`). Click **Commit changes**.

*(Prefer not to drag files in the browser? The free **GitHub Desktop** app makes this easier — or I can walk you through it screen-by-screen.)*

### Step 3: Connect Netlify
1. Go to **netlify.com** and sign up (choose "Sign up with GitHub" — easiest).
2. Click **Add new site → Import an existing project → GitHub**, and pick your `tbpe-website` repo.
3. Netlify automatically reads the build settings from `netlify.toml`. Just click **Deploy**.
4. In about a minute your site is live at a temporary address like `random-name-123.netlify.app`. 🎉

### Step 4: Turn on the editing panel (Identity)
1. In Netlify, open your site → **Site configuration → Identity → Enable Identity**.
2. Under **Identity → Services → Git Gateway**, click **Enable Git Gateway**.
3. Under **Identity → Registration**, set it to **Invite only** (so only your team can log in).
4. Click **Invite users**, enter your email, and send. Check your inbox and click the link to set a password.

### Step 5: Log in and edit
Go to **your-site-address/admin/** (e.g., `random-name-123.netlify.app/admin/`), log in, and you're in the editor. Every change you save publishes to the live site automatically in about a minute.

### Step 6: Connect your domain (when ready)
In Netlify → **Domain management → Add a domain** → enter `tampabaypropertyexperts.com`. Netlify shows you the DNS records to set at your domain registrar (where the domain is currently managed). Once DNS updates, your custom domain points to the new site. *(Tip: do Steps 1–5 first and confirm everything looks right before switching the live domain.)*

---

## Part 2 — How to edit (the everyday stuff)

Everything happens at **your-site/admin/**.

### Publish a blog post
1. Click **Blog Posts → New Blog Post**.
2. Fill in **Title**, **Publish date**, choose a **Category tag**, upload a **Thumbnail image**, write a one-line **Summary**, and write the **Article body** (it's a familiar rich-text/Markdown editor).
3. Click **Publish**. It appears on the Blog page automatically within ~1 minute. No code, no rebuilding by hand.

### Change your phone, email, address, or hours
**Site Settings → Contact & Business Info.** Edit and save — it updates across every page at once (header, footer, contact page).

### Change the homepage headline
**Site Settings → Homepage Hero.** Edit the heading, intro paragraph, or button labels and save.

### Add or change a photo in a blog post
Use the image button in the editor, or the Thumbnail field. Uploaded images are stored in `src/uploads` automatically.

---

## Part 3 — Still to wire up (when you're ready)

These are intentionally left as the final connections, because they need accounts created under your business identity:

1. **The forms** (Apply, Pay Rent, Maintenance, Contact, Rental Analysis) currently show a friendly "submitted!" confirmation but don't send anywhere yet. Easiest fix: turn on **Netlify Forms** (free tier) so submissions email you — or point Apply/Pay-Rent at your DoorLoop portal.
2. **DoorLoop** (recommended) for the real application + fee + screening (applicant self-enters SSN) and ACH rent. Once your account exists, the Apply and Pay Rent buttons link straight to it.
3. **Google Business Profile** — claim/optimize it for local search (see the strategy doc).
4. **A branded email** (e.g., info@tampabaypropertyexperts.com) to replace the personal address.

I can help set up any of these — including doing the GitHub + Netlify steps with you over a screen share using the browser tools, if you'd rather not do it solo.

---

## Quick reference

| I want to… | Where to go |
|---|---|
| Publish a blog post | `/admin` → Blog Posts → New |
| Change phone / email / address | `/admin` → Site Settings → Contact & Business Info |
| Edit the homepage headline | `/admin` → Site Settings → Homepage Hero |
| See the live site | your Netlify address (or your domain once connected) |
| Add team editors | Netlify → Identity → Invite users |

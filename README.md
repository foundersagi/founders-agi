# Founders AGI — Official Website

> Intelligence for Builders

**Live Site**: [https://YOUR_GITHUB_USERNAME.github.io/founders-agi](https://YOUR_GITHUB_USERNAME.github.io/founders-agi)

---

## 🚀 Deploy to GitHub Pages in 5 Minutes

### Step 1 — Create the Repository

1. Go to [github.com/new](https://github.com/new)
2. Name it `founders-agi` (or `YOUR_USERNAME.github.io` to use your root domain)
3. Set to **Public**
4. Click **Create repository**

### Step 2 — Upload Files

Upload these files to the root of your repository:
```
index.html        ← main website (required)
logo.png          ← your Founders AGI logo (required)
README.md         ← this file (optional)
```

**To upload your logo:**
1. Export your logo as `logo.png` (recommended: 200×200px, PNG with transparent background)
2. Upload it alongside `index.html`

### Step 3 — Enable GitHub Pages

1. Go to your repository → **Settings**
2. Scroll to **Pages** in the left sidebar
3. Under **Source**, select `Deploy from a branch`
4. Choose **main** branch → **/ (root)** folder
5. Click **Save**

Your site will be live at:
`https://YOUR_USERNAME.github.io/founders-agi`

(Takes 1–2 minutes to deploy)

---

## 📁 File Structure

```
founders-agi/
├── index.html      # Complete website (all-in-one)
├── logo.png        # Your logo
└── README.md       # This file
```

Everything is in a single `index.html` — no build tools, no dependencies, no npm needed.

---

## 🎨 Customizations

### Update your email
Search for `hello@foundersagi.com` and replace with your real email.

### Add your domain later
When you get a domain:
1. Go to Settings → Pages
2. Under **Custom domain**, enter your domain
3. Add a `CNAME` file to the repo with just your domain name (e.g., `foundersagi.com`)

### Update waitlist storage
Currently saves to browser localStorage for demo purposes. When you're ready for a real backend, replace the `submitWaitlist()` function in `index.html` with a call to:
- [Formspree](https://formspree.io) (free, simple)
- [Airtable API](https://airtable.com)
- Your own backend

**Formspree setup (easiest):**
1. Sign up at formspree.io
2. Create a form, get your endpoint (e.g. `https://formspree.io/f/XXXXX`)
3. Replace `submitWaitlist()` body with:
```js
fetch('https://formspree.io/f/XXXXX', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify({ name, email, stage, product })
});
```

---

## 🛠 Products Featured

| Product | Status | Description |
|---------|--------|-------------|
| FounderMind | Beta | AI co-founder for strategy & decisions |
| PitchForge | Coming Soon | AI pitch decks & financial models |
| LaunchOS | Coming Soon | Full launch kit in hours |
| MarketLens | Coming Soon | Market intelligence & competitor tracking |
| NetworkAGI | Coming Soon | AI-powered relationship & investor matching |
| BuilderAPI | Coming Soon | Founders AGI as infrastructure |

---

## 🔗 Links

- **LinkedIn**: https://www.linkedin.com/company/founders-agi-foundation/
- **Founder**: https://www.linkedin.com/in/chandan-sah-rocky-文浩-5803bb1b4/

---

Built with 🔥 by Chandan Sah Rocky · © 2025 Founders AGI Foundation

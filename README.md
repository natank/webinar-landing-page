# Webinar Landing Page

Promotional landing page for the **AI-Assisted Software Development** webinar,
deployed to GitHub Pages.

## Deploying to GitHub Pages

### Prerequisites
- A GitHub account with access to `git@github.com:natank/webinar-landing-page.git`
- Git installed locally

### Steps

#### 1. Clone / push to the repository

If starting fresh:
```bash
cd /path/to/webinar-landing-page
git init
git add .
git commit -m "Initial landing page"
git remote add origin git@github.com:natank/webinar-landing-page.git
git push -u origin main
```

#### 2. Enable GitHub Pages

1. Go to the repository on GitHub → **Settings** → **Pages** (left sidebar).
2. Under **Source**, select **Deploy from a branch**.
3. Choose branch `main` and folder `/ (root)`.
4. Click **Save**.

GitHub will build and publish the page. The URL will be:
```
https://natank.github.io/webinar-landing-page/
```

It may take 1–2 minutes for the first deploy to appear.

#### 3. Verify the deployment

Open the URL above in a browser. If you see the landing page, you're done.

### Updating the page

1. Edit `index.html`.
2. Commit and push:
   ```bash
   git add index.html
   git commit -m "Update landing page"
   git push
   ```
3. GitHub Pages re-deploys automatically within ~1 minute.

## Customising before go-live

| Item | Where to edit |
|------|--------------|
| Webinar date & time | `index.html` — `.meta-bar` section |
| Google Form link | `index.html` — `href` on the `.register-link` anchor (replace `PLACEHOLDER_FORM_ID`) |
| Speaker / presenter info | Add a new section after `#audience` |
| Colors / branding | `index.html` — CSS `:root` variables |

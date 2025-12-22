# Mintlify Setup Guide for Okasie Partner API Docs

This guide walks you through setting up the Okasie Partner API documentation on Mintlify.

---

## Quick Setup (5 minutes)

### Step 1: Create a Mintlify Project

1. Go to [mintlify.com](https://mintlify.com) and sign in
2. Click **"New Project"** or **"Create Documentation"**
3. Choose **"Start from scratch"** or connect to a GitHub repo

### Step 2: Upload/Paste the Configuration

In Mintlify's editor, create/update `docs.json` with the configuration from this folder.

**Option A: GitHub Integration (Recommended)**
- Connect your GitHub repo to Mintlify
- Push the entire `/docs` folder to your repo
- Mintlify will automatically deploy

**Option B: Manual Upload**
- Copy each file from this `/docs` folder into Mintlify's web editor

### Step 3: Add Your Logo

1. Download your Okasie logo (SVG format preferred)
2. Upload to `/logo/dark.svg` and `/logo/light.svg`
3. Or update the `docs.json` to point to external URLs

### Step 4: Configure Your Domain

1. In Mintlify Dashboard → Settings → Custom Domain
2. Add `docs.okasie.be` (or your preferred subdomain)
3. Follow DNS configuration instructions

---

## File Overview

| File | Purpose | Copy to Mintlify |
|------|---------|------------------|
| `docs.json` | Main configuration | Yes - root level |
| `openapi.yaml` | API specification | Yes - root level |
| `introduction.mdx` | Welcome page | Yes - root level |
| `quickstart.mdx` | Getting started | Yes - root level |
| `authentication.mdx` | Auth guide | Yes - root level |
| `rate-limiting.mdx` | Rate limits | Yes - root level |
| `errors.mdx` | Error codes | Yes - root level |
| `api-reference/*.mdx` | API endpoints | Yes - keep folder structure |
| `guides/*.mdx` | Tutorials | Yes - keep folder structure |
| `nl/*.mdx` | Dutch translations | Yes - keep folder structure |

---

## Local Preview

To preview the documentation locally before deploying:

```bash
# Install Mintlify CLI
npm i -g mintlify

# Navigate to docs folder
cd /path/to/okasie/docs

# Start local preview
mintlify dev
```

Open http://localhost:3000 to see your docs.

---

## Deployment Checklist

- [ ] Upload `docs.json` configuration
- [ ] Upload `openapi.yaml` specification
- [ ] Create all MDX pages
- [ ] Add logo files (or update URLs in docs.json)
- [ ] Configure custom domain (optional)
- [ ] Test API playground with your API key

---

## Support

- Mintlify docs: https://mintlify.com/docs
- Okasie support: info@okasie.be

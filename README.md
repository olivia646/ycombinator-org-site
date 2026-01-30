# YCombinator.org

Public-facing website for the Y Combinator International Founder Award, administered by YCombinator.org, a California 501(c)(3) nonprofit organization.

## About

The Y Combinator International Founder Award is a non-monetary credential recognizing exceptional entrepreneurial achievement among non-U.S. founders accepted into Y Combinator's accelerator program.

**YCombinator.org** is a DBA (Doing Business As) of **YC ORG** (EIN: 47-3772053).

## Tech Stack

- Pure HTML/CSS/JS (no framework dependencies)
- Mobile-responsive design
- Optimized for fast loading and SEO

## Deployment to Vercel

### Option 1: Deploy via GitHub (Recommended)

1. **Create a new GitHub repository:**
   ```bash
   # Initialize git in the project folder
   git init
   git add .
   git commit -m "Initial commit: YCombinator.org website"
   
   # Create repo on GitHub, then:
   git remote add origin https://github.com/YOUR_USERNAME/ycombinator-org.git
   git branch -M main
   git push -u origin main
   ```

2. **Connect to Vercel:**
   - Go to [vercel.com](https://vercel.com)
   - Click "Add New Project"
   - Import your GitHub repository
   - Keep default settings (Vercel auto-detects static sites)
   - Click "Deploy"

3. **Configure custom domain:**
   - In Vercel project settings → Domains
   - Add `ycombinator.org`
   - Update your domain's DNS records as instructed by Vercel

### Option 2: Deploy via Vercel CLI

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy (from project directory)
vercel

# Deploy to production
vercel --prod
```

## Local Development

Simply open `index.html` in a browser, or use a local server:

```bash
# Using Python (run from your system terminal, e.g. Terminal.app)
python3 -m http.server 8080
```

Then visit **http://localhost:8080** (or http://127.0.0.1:8080).

**If the browser can't connect:** Run the command above in **Terminal.app** (or another system terminal), not from Cursor’s background or a sandboxed environment. Sandboxed environments can block binding to ports with `PermissionError: [Errno 1] Operation not permitted`.

Other options (also run from a normal terminal):

```bash
# Node.js
npx serve

# PHP
php -S localhost:8080
```

## File Structure

```
ycombinator-org/
├── index.html      # Main HTML file
├── styles.css      # All styles
└── README.md       # This file
```

## Customization

### Colors
Edit CSS variables in `styles.css`:
```css
:root {
    --yc-orange: #FF6600;
    --text-primary: #1A1A1A;
    --text-secondary: #666666;
    /* ... */
}
```

### Content
All content is in `index.html`. Edit the text directly in the HTML sections.

## Legal

- **Organization:** YCombinator.org
- **Type:** California 501(c)(3) nonprofit
- **EIN:** 47-3772053
- **Address:** 335 Pioneer Way, Mountain View, CA 94041

---

© 2025 YCombinator.org. All rights reserved.

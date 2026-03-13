# Atlas Trade Intelligence

Global Trade & Financial Clearance Platform — static HTML site ready for Vercel.

## Deploy to Vercel (2 minutes)

### Option A — Vercel CLI (fastest)
```bash
# 1. Install Vercel CLI
npm install -g vercel

# 2. Navigate into this folder
cd atlas-trade-vercel

# 3. Deploy
vercel

# Follow the prompts:
#   Set up and deploy? → Y
#   Which scope? → your account
#   Link to existing project? → N
#   Project name → atlas-trade-intelligence (or any name)
#   In which directory is your code? → ./
#   Want to override settings? → N
```
Your live URL will be printed instantly (e.g. https://atlas-trade-intelligence.vercel.app)

### Option B — Drag & Drop (zero setup)
1. Go to https://vercel.com/new
2. Click **"Import Third-Party Git Repository"** or drag this folder
3. Or use **"Deploy from template"** → drop the folder
4. Done — live in ~30 seconds

### Option C — GitHub (recommended for ongoing updates)
1. Create a new GitHub repo
2. Push this folder to it:
   ```bash
   git init
   git add .
   git commit -m "Initial deploy"
   git remote add origin https://github.com/YOUR_USERNAME/atlas-trade.git
   git push -u origin main
   ```
3. Go to https://vercel.com/new → Import your GitHub repo
4. Vercel auto-detects static site → click Deploy

## Project Structure
```
atlas-trade-vercel/
├── public/
│   └── index.html        ← The entire website (self-contained)
├── vercel.json           ← Vercel config + security headers
├── package.json
├── .gitignore
└── README.md
```

## Custom Domain (after deploy)
1. In Vercel dashboard → your project → Settings → Domains
2. Add your domain (e.g. atlastrade.io)
3. Update your DNS with the CNAME/A records Vercel shows you

## Local Preview
```bash
npx serve public -p 3000
# Open http://localhost:3000
```

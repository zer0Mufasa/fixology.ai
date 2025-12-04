# Fixology Website - Complete Documentation

## 📁 Project Structure

```
fixology-v2/
├── public/
│   ├── index.html          # Homepage
│   ├── diagnose.html       # Customer diagnosis page
│   ├── for-shops.html      # SaaS landing page
│   ├── pricing.html        # Pricing page
│   ├── learn.html          # Education hub
│   ├── about.html          # About/story page
│   ├── login.html          # Login portal
│   ├── partners.html       # Partner program
│   ├── contact.html        # Contact form
│   ├── results.html        # Sample diagnosis results
│   ├── privacy.html        # Privacy policy
│   ├── terms.html          # Terms of service
│   └── vercel.json         # Vercel configuration
├── dashboard/
│   └── preview.html        # SaaS dashboard preview
├── DESIGN-SYSTEM.md        # Design documentation
└── README.md               # This file
```

---

## 🗺️ Sitemap

### Public Pages
| URL | Page | Description |
|-----|------|-------------|
| `/` | Homepage | Main landing, hero, features, testimonials |
| `/diagnose` | Diagnose | Customer AI diagnosis interface |
| `/for-shops` | For Shops | SaaS platform landing page |
| `/pricing` | Pricing | Customer & shop pricing tiers |
| `/learn` | Learn | Educational articles hub |
| `/about` | About | Company story, founder, roadmap |
| `/login` | Login | Shop portal / customer login |
| `/partners` | Partners | Partner shop program |
| `/contact` | Contact | Contact form |
| `/results` | Results | Sample diagnosis mockup |
| `/privacy` | Privacy | Privacy policy |
| `/terms` | Terms | Terms of service |
| `/dashboard` | Dashboard | SaaS dashboard preview |

---

## 🚀 Deployment Guide

### Option 1: Vercel (Recommended)

1. **Push to GitHub**
   ```bash
   cd fixology-v2
   git init
   git add .
   git commit -m "Initial Fixology v2 website"
   git remote add origin https://github.com/YOUR_USERNAME/fixology-website.git
   git push -u origin main
   ```

2. **Connect to Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Import your GitHub repository
   - Set root directory to `public`
   - Deploy

3. **Custom Domain**
   - In Vercel dashboard → Settings → Domains
   - Add `fixologyai.com`
   - Configure DNS:
     - A Record: `@` → `76.76.21.21`
     - CNAME: `www` → `cname.vercel-dns.com`

### Option 2: Netlify

1. Push to GitHub
2. Connect repo to Netlify
3. Set publish directory to `public`
4. Configure redirects in `_redirects` file

### Option 3: Manual Hosting

Upload contents of `public/` to any static hosting:
- AWS S3 + CloudFront
- Google Cloud Storage
- DigitalOcean Spaces
- Any Apache/Nginx server

---

## 🔧 Configuration

### vercel.json
The Vercel config enables:
- Clean URLs (no .html extensions)
- Security headers
- URL rewrites for all pages

### DNS Records (for fixologyai.com)
```
Type    Name    Value
A       @       76.76.21.21
CNAME   www     cname.vercel-dns.com
```

---

## 📊 Pages Overview

### Homepage (`index.html`)
- Hero with animated gradient background
- "How It Works" 4-step process
- Dual value prop (customers + shops)
- 9 feature cards
- Diagnostic preview mockup
- 3 testimonials
- FAQ accordion
- CTA section
- Full footer

### Diagnose Page (`diagnose.html`)
- Hero explaining the service
- Example prompt chips
- Chat interface mockup
- Link to live GPT bot
- Info cards (free, instant, private)
- Safety warning section

### For Shops (`for-shops.html`)
- Hero with dashboard preview
- 6 benefit cards
- 12 feature cards
- 3 pricing tiers preview
- Early access application form

### Pricing Page (`pricing.html`)
- Customer pricing (free + $5 report)
- Shop pricing (3 tiers)
- Commission model explanation
- FAQ accordion

### Learn Page (`learn.html`)
- Category filter tabs
- 8 article cards
- Featured guide section
- CTA to diagnose

### About Page (`about.html`)
- Founder story
- "The Problem" narrative
- Founder card (Mustafa)
- 4 values cards
- Stats display
- Roadmap (3 phases)

### Partners Page (`partners.html`)
- 6 benefits
- 4-step process
- Requirements (what you need / don't need)
- Partner application form

### Dashboard Preview (`dashboard/preview.html`)
- Full sidebar navigation
- Stats grid (4 KPIs)
- Recent tickets table
- Alerts section
- Activity feed
- Preview banner with CTA

---

## 🎨 Brand Guidelines

### Colors
- Primary: Lavender gradient (#B48FFF → #8E75FF → #6B59FF)
- Accent: Neon cyan (#6DF7FF)
- Background: Near-black (#07070A)
- Text: White → Gray scale

### Typography
- Font: Inter (Google Fonts)
- Headings: Bold, tight letter-spacing
- Body: Regular, 15px base

### Voice & Tone
- **Calm**: Not hype, not salesy
- **Confident**: We know repair
- **Direct**: Clear and concise
- **Trustworthy**: Built by real techs

### Visual Style
- Clean, minimal design
- Generous whitespace
- Subtle gradients and glows
- Dark mode only
- Emoji icons

---

## 🔌 Integrations

### Current
- **OpenAI GPT**: Customer diagnosis bot
  - URL: `https://chatgpt.com/g/g-692e842d0dc48191989c1f877d00165d-fixology-repair-assistant`
- **Notion**: Knowledge graph database

### Planned
- **Supabase**: User auth & database
- **Stripe**: Payment processing
- **Twilio**: SMS notifications
- **Google Maps**: Shop locations
- **Analytics**: Plausible or Fathom

---

## 💰 Monetization Summary

### B2C (Customers)
- Free AI diagnosis
- $5 detailed report (coming soon)
- Commission from shop referrals

### B2B (Repair Shops)
| Tier | Price | Features |
|------|-------|----------|
| Starter | $0/mo | 50 diagnoses, basic ticketing |
| Pro | $99/mo | Unlimited, full POS, chatbot, training |
| Enterprise | Custom | Multi-location, API, white-label |

### Referral Commission
- 10-20% of repair revenue from Fixology-referred customers

---

## 📈 Next Steps

### Phase 1 (Current)
- [x] Complete website redesign
- [x] All public pages created
- [x] Dashboard preview
- [ ] Deploy to Vercel
- [ ] Connect custom domain
- [ ] Form backend (Formspree/Notion)

### Phase 2 (Q1 2025)
- [ ] User authentication
- [ ] Shop dashboard (functional)
- [ ] POS system
- [ ] Inventory management
- [ ] Stripe integration

### Phase 3 (Q2 2025)
- [ ] Multi-store support
- [ ] Android device support
- [ ] Parts marketplace
- [ ] API for chains
- [ ] Mobile app

---

## 📞 Support

- Email: hello@fixologyai.com
- Website: fixologyai.com
- GitHub: github.com/fixology

---

*Built with 💜 by Mustafa in Missouri*

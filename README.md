# Functionally Fitness Website

Science-based personal training website for Functionally Fitness, a one-on-one coaching business serving the Clarksville, TN and Fort Campbell areas with evidence-driven programming and professional coaching.

**Live Site**: [functionallyfitness.com](https://functionallyfitness.com)

---

## Quick Start

### For Deployment
```bash
# After making changes locally
git add .
git commit -m "Your clear commit message"
git push origin main
# Cloudflare Pages auto-deploys within minutes
```

### For Local Testing
1. Open `index.html` in any modern web browser
2. Test all links and responsive design by resizing your browser
3. Changes are instant—no build step required

---

## Project Structure

```
functionally-fitness/
├── index.html              ← Main website (all-in-one, no external dependencies)
├── README.md               ← This file
├── IMAGE_GUIDE.md          ← Detailed image asset naming and placement guide
├── .gitignore              ← Git configuration
├── css/                    ← (Can be deleted—CSS is now embedded in index.html)
│   └── style.css
└── images/                 ← Image assets (see IMAGE_GUIDE.md for details)
    ├── logo.png                    ✓ Keep
    ├── download.jpg                ← Hero background image
    ├── tyler-smith-coach.jpg       ← Coach profile image
    ├── in-person-training.jpg      ← Service card 1
    ├── online-coaching.jpg         ← Service card 2
    ├── hybrid-training.jpg         ← Service card 3
    └── specialized-programs.jpg    ← Service card 4
```

---

## Design System

### Brand Colors
- **Primary (Forest Green)**: `#1B4332` — Hero sections, text, accents
- **Secondary (Teal)**: `#2A9D8F` — Buttons, borders, hover states
- **Accent (Gold)**: `#B08D57` — Highlights, decorative elements, premium feel
- **Background (Cream)**: `#faf8f5` — Main page background, card interiors

### Typography
- **Headings**: Cinzel (serif) — weights 400, 600, 700, 900
- **Body**: Cormorant Garamond (serif) — weights 400, 500, 600, 700
- **Fallback**: System serif fonts if Google Fonts unavailable

### Aesthetic
- **Art Deco inspired** with subtle 2px borders and CSS ::after corner accents
- **Rounded 2px corners** for modern minimalism
- **Gradient overlays** on hero and portal sections
- **Box shadows** for depth and layering
- **Smooth transitions** (0.3s ease) on all interactive elements

---

## Website Sections

1. **Header** (Sticky)
   - Logo and business name
   - Navigation menu: Why Us, Meet Tyler, Services, Plans
   - Client Portal button and Book Now CTA

2. **Hero Section**
   - Full-screen background image (download.jpg)
   - Semi-transparent overlay gradient for text readability
   - Main value proposition: "Science-Based Personal Training"
   - Free Consultation booking link

3. **Methodology** — "Our Science-Based Approach"
   - 4-step process cards: Assessment → Programming → Execution → Progression
   - Educational content about training philosophy

4. **Expertise** — "Professional Credentials"
   - 8 certification grid: NASM-PES, NASM-CPT, ISSA-CES, PhysioCore, Precision Nutrition, FMS Level 2, Exercise Science, Continued Learning
   - Reinforces credibility and specialization

5. **Coach Profile** — "Meet Tyler Smith"
   - High-quality coach portrait (tyler-smith-coach.jpg)
   - Background and philosophy
   - List of specializations
   - Builds trust and personal connection

6. **Training Services** — 4 Options with Images
   - In-Person Sessions (in-person-training.jpg)
   - Online Coaching (online-coaching.jpg)
   - Hybrid Training (hybrid-training.jpg)
   - Specialized Programs (specialized-programs.jpg)
   - Each card links to appropriate intake form or booking

7. **Pricing Plans** — 3 Tiers
   - **Starter** ($99/mo) — 2 sessions/month, basic features
   - **Pro** ($249/mo) — Unlimited sessions, most popular, featured badge
   - **Elite** ($499/mo) — Premium tier with advanced recovery protocols
   - Each tier links to relevant Jotform intake

8. **Client Portal** — Gradient Section
   - Features grid: Progress Tracking, Workout Access, Session Booking, Direct Messaging
   - Direct link to https://portal.functionallyfitness.com
   - Gradient background (primary to secondary color)

9. **Contact Section**
   - Main CTA to book free consultation
   - Contact methods: Phone, Location, Email
   - Card-based layout matching design system

10. **Footer**
    - Copyright notice
    - Social media links

---

## Key Links & External Services

### Booking & Forms
- **Free Consultation Calendar**: https://calendar.app.google/uceB14mhh3rDk57X7
- **Client Portal**: https://ffclientportal.floot.app

### Tier Intake Forms (Jotform)
- **Tier 1 Intake**: https://form.jotform.com/262446754363059
- **Tier 2 Intake**: https://form.jotform.com/262446601203043
- **Tier 3 Intake**: https://form.jotform.com/262447336815058

### Contact Information
- **Phone**: (719) 963-2122 (with tel: link for mobile)
- **Location**: Clarksville, TN & Fort Campbell Areas
- **Email**: functionallyfitness@gmail.com

---

## Image Assets & Specifications

**Complete guide in IMAGE_GUIDE.md**. Quick summary:

| Filename | Purpose | Dimensions | Notes |
|----------|---------|------------|-------|
| `logo.png` | Header logo | ~50px height | Transparent PNG recommended |
| `download.jpg` | Hero background | 1920×1080+ | 16:9 ratio, semi-transparent overlay |
| `tyler-smith-coach.jpg` | Coach profile | ~500×600px | Portrait orientation |
| `in-person-training.jpg` | Service card 1 | 400×280px | Dumbbells/gym setting |
| `online-coaching.jpg` | Service card 2 | 400×280px | Remote/athlete training |
| `hybrid-training.jpg` | Service card 3 | 400×280px | Mixed modality training |
| `specialized-programs.jpg` | Service card 4 | 400×280px | Advanced/athlete training |

**Optimization Tips**:
- Save JPGs at 80-85% quality
- Use TinyPNG or ImageOptim to compress
- Target file sizes: 200-400KB per image

---

## Customization Guide

### Updating Contact Information
Edit the contact section in `index.html`:
```html
<a href="tel:7199632122">(719) 963-2122</a>
<p>Clarksville, TN & Fort Campbell Areas</p>
<p><a href="mailto:contact@functionallyfitness.com">contact@functionallyfitness.com</a></p>
```

### Changing Brand Colors
Modify CSS variables at the top of `<style>`:
```css
:root {
    --primary-color: #1B4332;
    --secondary-color: #2A9D8F;
    --accent-color: #B08D57;
    --cream-bg: #faf8f5;
}
```

### Updating Business Links
Search for these URLs in `index.html` and replace:
- Google Calendar: `https://calendar.app.google/uceB14mhh3rDk57X7`
- Jotform links: Replace all three form URLs
- Client Portal: `https://ffclientportal.floot.app`

### Adding New Sections
1. Add HTML markup in `<body>`
2. Add corresponding CSS styles in `<style>`
3. Use existing color variables for consistency
4. Test responsive design (768px, 480px breakpoints)

---

## Deployment

### Automatic Deployment (Recommended)
This site is configured for **Cloudflare Pages** auto-deployment:
1. Push changes to GitHub (`git push origin main`)
2. Cloudflare automatically builds and deploys within 1-5 minutes
3. Changes live at functionallyfitness.com

### Manual Deployment Checklist
- [ ] All images optimized and in `/images/` folder
- [ ] Filenames match exactly (case-sensitive on Linux)
- [ ] All external links updated and tested
- [ ] Responsive design verified (mobile/tablet/desktop)
- [ ] Changes committed with clear message
- [ ] Pushed to GitHub main branch
- [ ] Cloudflare deployment triggered

### Troubleshooting Deployment

**Images not showing:**
- Verify filenames match exactly (case-sensitive)
- Check that images were added to git: `git add images/`
- Clear browser cache: Ctrl+Shift+Delete (Cmd+Shift+Delete on Mac)
- Hard refresh: Ctrl+Shift+R (Cmd+Shift+R on Mac)
- Purge Cloudflare cache from dashboard

**Changes not live:**
- Verify commit pushed: `git log` shows your commits
- Check Cloudflare Pages dashboard for deployment status
- Wait 5-10 minutes for full propagation
- Try incognito/private browser window

**Styling issues:**
- CSS is embedded directly in `index.html` (no external files)
- Clear browser cache if recent changes not showing
- Check browser console for JavaScript errors (F12 key)

---

## Development Notes

- **No build process required** — this is a static HTML website
- **No JavaScript framework** — vanilla HTML/CSS for maximum performance
- **Embedded CSS** — all styling in `<style>` tag for reliability
- **Google Fonts** — imported via `@import url()` for fallback support
- **Responsive design** — Mobile-first approach with 768px and 480px breakpoints

### Local Development
```bash
# Option 1: Open file directly
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux

# Option 2: Use a local server (Python 3)
python -m http.server 8000
# Then visit http://localhost:8000
```

---

## Maintenance & Updates

### Regular Maintenance Tasks
- **Monthly**: Review contact information, links, and forms
- **Quarterly**: Check image optimization and file sizes
- **As needed**: Update credentials, services, or pricing

### Version Control Workflow
```bash
# See your changes
git status

# Stage all changes
git add .

# Commit with descriptive message
git commit -m "Clear description of what changed"

# Push to GitHub (triggers Cloudflare deployment)
git push origin main

# Verify deployment
# Visit functionallyfitness.com in browser
```

### Git Commit Message Examples
```
Add new coach photo and update credentials
Update pricing for Elite tier
Fix typo in methodology section
Add new service offering
Update contact phone number
```

---

## Performance & Best Practices

- **Page load**: ~1-2 seconds (depends on image optimization)
- **Mobile responsive**: Optimized for 320px+ widths
- **Accessibility**: Semantic HTML, alt text on all images
- **SEO**: Title tag, meta description, semantic structure

### Optimization Tips
- Keep images under 400KB each
- Use 16:9 aspect ratio for hero image
- Test on real devices (not just browser resize)
- Monitor Cloudflare analytics for performance metrics

---

## Browser Support

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

---

## FAQ

**Q: How long does deployment take?**  
A: Typically 1-5 minutes after pushing to GitHub. Cloudflare Pages handles everything automatically.

**Q: Can I edit the website without coding?**  
A: You'll need basic text editing knowledge to update content. HTML and CSS are in one file. If you're uncomfortable editing, reach out with your desired changes.

**Q: What if images aren't showing?**  
A: See "Troubleshooting Deployment" section above. Most issues are filename or caching related.

**Q: Can I change the colors?**  
A: Yes! Edit the CSS variables at the top of `<style>`. See "Customization Guide" for details.

**Q: How do I add a new section?**  
A: Add HTML markup in the body, add CSS styles, and test responsive design. Follow existing section patterns for consistency.

---

## Support & Contact

For website issues, updates, or questions about the deployment:
- Review IMAGE_GUIDE.md for asset management
- Check this README for common issues
- Consult the "Customization Guide" for making changes
- Test locally in `index.html` before committing

**Business Contact**:
- Phone: (719) 963-2122
- Email: functionallyfitness@gmail.com
- Location: Clarksville, TN & Fort Campbell Areas

---

## License & Copyright

© 2024 Functionally Fitness. All rights reserved.

Website design and deployment: Cloudflare Pages

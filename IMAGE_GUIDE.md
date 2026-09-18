# Image Asset Guide for Functionally Fitness Website

## Overview
The redesigned website now integrates 7 high-quality fitness photography images throughout the design. Below is the complete guide for organizing and naming your images.

## Required Images & Placement

### 1. **logo.png** (Already in place)
- **Purpose:** Header logo displayed at top-left
- **Dimensions:** Any (will scale to 50px height)
- **Current file:** ✓ Already exists in images/ folder
- **Notes:** Teal crown logo in #2A9D8F color

### 2. **download.jpg** (Header/Hero Background)
- **Purpose:** Full-screen hero section background image
- **Placement:** Hero section background (top of page)
- **Dimensions:** Recommended 1920x1080px or similar 16:9 ratio
- **Usage:** Applied with semi-transparent overlay (dark green + teal gradient) for text readability
- **Status:** ⚠️ NEEDS TO BE ADDED
- **File location:** `/images/download.jpg`

### 3. **tyler-smith-coach.jpg** (Coach Profile)
- **Purpose:** Coach profile image in "Meet Tyler Smith" section
- **Placement:** Left side of coach section (medium section)
- **Dimensions:** Recommended 500x600px or similar portrait orientation
- **Styling:** 3px gold border, box shadow, object-fit: cover
- **Status:** ⚠️ NEEDS TO BE ADDED
- **File location:** `/images/tyler-smith-coach.jpg`
- **Notes:** Portrait-oriented image of Tyler Smith as the coach/founder

### 4. **in-person-training.jpg** (Service Card 1)
- **Purpose:** In-Person Sessions training card image
- **Placement:** First card in Training Services grid
- **Dimensions:** Recommended 400x280px (or maintain aspect ratio)
- **Styling:** 280px height with object-fit: cover
- **Status:** ⚠️ NEEDS TO BE ADDED
- **File location:** `/images/in-person-training.jpg`
- **Notes:** Image showing in-person training (dumbbells, equipment, or gym setting)

### 5. **online-coaching.jpg** (Service Card 2)
- **Purpose:** Online Coaching training card image
- **Placement:** Second card in Training Services grid
- **Dimensions:** Recommended 400x280px (or maintain aspect ratio)
- **Styling:** 280px height with object-fit: cover
- **Status:** ⚠️ NEEDS TO BE ADDED
- **File location:** `/images/online-coaching.jpg`
- **Notes:** Image showing online coaching (athlete, screen, or remote training)

### 6. **hybrid-training.jpg** (Service Card 3)
- **Purpose:** Hybrid Training Programs card image
- **Placement:** Third card in Training Services grid
- **Dimensions:** Recommended 400x280px (or maintain aspect ratio)
- **Styling:** 280px height with object-fit: cover
- **Status:** ⚠️ NEEDS TO BE ADDED
- **File location:** `/images/hybrid-training.jpg`
- **Notes:** Image showing mixed training modality (athlete training)

### 7. **specialized-programs.jpg** (Service Card 4)
- **Purpose:** Specialized Programs card image
- **Placement:** Fourth card in Training Services grid
- **Dimensions:** Recommended 400x280px (or maintain aspect ratio)
- **Styling:** 280px height with object-fit: cover
- **Status:** ⚠️ NEEDS TO BE ADDED
- **File location:** `/images/specialized-programs.jpg`
- **Notes:** Image showing specialized training (athlete, equipment, or advanced training)

## Complete Folder Structure

```
functionally-fitness/
├── images/
│   ├── logo.png                    ✓ (existing)
│   ├── download.jpg                (new - hero background)
│   ├── tyler-smith-coach.jpg       (new - coach profile)
│   ├── in-person-training.jpg      (new - service card 1)
│   ├── online-coaching.jpg         (new - service card 2)
│   ├── hybrid-training.jpg         (new - service card 3)
│   └── specialized-programs.jpg    (new - service card 4)
├── index.html                       (updated with new design)
├── .gitignore
├── README.md
└── IMAGE_GUIDE.md                   (this file)
```

## Implementation Steps

1. **Rename your image files** to match the names above exactly
2. **Copy all images** into the `/images/` folder
3. **Replace** the old `images/` folder contents with the new files
4. **Test locally** by opening index.html in your browser
5. **Commit and push** to GitHub to deploy via Cloudflare Pages

```bash
# Git workflow
git add images/
git add index.html
git commit -m "Add photography assets and redesigned layout"
git push origin main
```

## Image Quality Recommendations

- **Format:** JPG for photographs (better compression), PNG for logo/graphics
- **Quality:** Save JPGs at 80-85% quality for optimal file size and quality balance
- **Optimization:** Consider using tools like TinyPNG or ImageOptim to reduce file sizes
- **Sizing:** Optimize to actual display size to reduce load time

## Design Notes

- All images use `object-fit: cover` for consistent card heights regardless of image dimensions
- Hero section uses a semi-transparent overlay (gradient) over the background image for text readability
- Service card images are displayed at 280px height with automatic width scaling
- Coach profile image maintains aspect ratio with responsive sizing

## Deployment Checklist

- [ ] All 7 images properly named and placed in `/images/` folder
- [ ] Images optimized for web (reasonable file sizes)
- [ ] `index.html` updated and testing locally shows all images
- [ ] Changes committed to git with clear message
- [ ] Pushed to GitHub main branch
- [ ] Cloudflare Pages deployment triggered and live site updated
- [ ] Live website displays all images correctly
- [ ] All buttons and links working properly
- [ ] Responsive design verified on mobile/tablet/desktop

## Troubleshooting

**Images not showing on live site:**
- Clear browser cache (Ctrl+Shift+Delete or Cmd+Shift+Delete)
- Verify file names match exactly (case-sensitive on Linux servers)
- Check that files were added to git and committed
- Hard refresh: Ctrl+Shift+R or Cmd+Shift+R
- Purge Cloudflare cache from dashboard if still not showing

**Images look stretched/distorted:**
- Check image dimensions and aspect ratios
- The CSS uses `object-fit: cover` which maintains aspect ratio
- Ensure images are not excessively small

**File size concerns:**
- Consider optimizing images before uploading
- Aim for 200-400KB per image file maximum
- Use modern formats (WebP as alternative if browser support needed)

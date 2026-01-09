# Dr. Juan Palomar Tribute Page

## Project Overview
A single-page scrolling tribute to Dr. Juan Manuel Palomar, MD (1948-2018), a pioneer in Pediatric Urology who died from a brain tumor caused by decades of occupational radiation exposure from fluoroscopy procedures.

**Live URL:** https://juan-palomar-tribute.orsif.org

**GitHub:** https://github.com/screendoorstudio/orsif-juan-palomar

## Key People
- **Dr. Juan Manuel Palomar** - The subject of the tribute
- **Nola Palomar** - Juan's wife, provided photos, story content, and YouTube video
- **Bob Foster, MD** - ORSIF/Rampart founder who initiated this tribute project

## Design Decisions

### "Warmer as You Scroll"
The page transitions emotionally from professional/clinical at the top to warm/personal at the bottom:
- **Top:** Dark teal ORSIF branding (#0d4d5f), professional medical context
- **Middle:** Story unfolds, warmer colors begin appearing
- **Bottom:** Warm amber/gold tones (#d4a574, #faf8f5), personal photos, celebration of life

### Single-Page Scroller
- No navigation menu - just minimal header with ORSIF logo and "Join ORSIF" CTA
- Smooth scroll through all sections
- Fade-in animations on scroll

## Page Sections
1. **Minimal Header Bar** - ORSIF logo + Join button (sticky)
2. **Hero** - Compact section with teal line art of Juan on left, memorial text on right. Background uses gradient overlay on scrubs photo. Section height fits content (image flush with bottom).
3. **Short Story** - Word-for-word from Nola's provided content
4. **Full Story** - Timeline format with detailed narrative
5. **Video Tribute** - YouTube embed from Nola Palomar
6. **Winery Section** - Dominio Buenavista, his passion for wine
7. **Personal Section** - Family info + obituary link
8. **Why It Matters** - ORSIF mission connection, statistics
9. **CTA + Footer** - Join ORSIF call-to-action

## Content Sources

### Story Text
Both short and long versions came from `Juans Story.pdf` - an email from Nola Palomar to Bob Foster dated January 8, 2026. The text was used **word-for-word** as requested.

### Photos
Three photos provided by Nola Palomar:
- `Dr Palomar 1.jpg` - In blue scrubs at hospital (hero background)
- `Dr Palomar 2.jpg` - Close-up portrait with glasses (personal section)
- `Dr Palomar 3.JPG` - At Dominio Buenavista winery (winery section)

Photo credit for winery photo: Warren Dyer

### Video
YouTube video tribute from Nola Palomar:
- URL: https://www.youtube.com/watch?v=kTCtHHU0H9w
- Embedded in "Hear From Those Who Loved Him" section

### Obituary
Full obituary with additional photos: https://www.dignitymemorial.com/obituaries/dayton-oh/juan-palomar-7868104

## Technical Stack
- **HTML/CSS/JS** - Static site, no build process
- **Hosting:** Vercel
- **Domain:** juan-palomar-tribute.orsif.org (CNAME to cname.vercel-dns.com)
- **Repository:** GitHub (screendoorstudio/orsif-juan-palomar)

## File Structure
```
/
├── index.html              # Main tribute page
├── css/
│   └── styles.css          # ORSIF design system + warm transitions
├── js/
│   └── app.js              # Scroll animations, fade-in effects
├── images/
│   ├── Dr Palomar 1.jpg    # Scrubs photo (hero background)
│   ├── Dr Palomar 2.jpg    # Portrait (personal section)
│   ├── Dr Palomar 3.JPG    # Winery photo
│   ├── Juan-Palomar_line-art.png  # Teal line art illustration (hero section)
│   ├── orsif_logo_white.png
│   └── orsif_logo_tagline_white.png
├── screenshots/            # Development reference screenshots
├── .gitignore
└── claude.md               # This file
```

## ORSIF Design System Reference
Colors and styling match other ORSIF properties:
- Primary teal: #0d4d5f
- CTA green: #27ae60
- Font: System fonts (Apple, Segoe UI, Roboto)
- Headings: Georgia serif for warmth

Referenced existing ORSIF pages at:
- https://faqs.orsif.org
- https://guidelines-us.orsif.org
- https://guidelines-international.orsif.org

## Key Statistics (from ORSIF research)
Used in "Why It Matters" section:
- 85% of brain tumors in interventional cardiologists occur on the left side
- 6.1% lifetime cancer incidence rate
- 50% dosimeter non-compliance among physicians

## Recent Updates (January 2026)

### Hero Section Redesign
- Added teal line art illustration (`Juan-Palomar_line-art.png`) to left of memorial text
- Changed from full-viewport height to compact layout
- Image and text align at bottom (flex-end)
- Section bottom is flush with Juan's feet in the illustration
- Removed scroll indicator (no longer needed with shorter section)

### Hero Section CSS Details
- Background: Gradient overlay on `Dr Palomar 1.jpg`
- Gradient colors: `rgba(13, 77, 95, 0.92)` to `rgba(9, 58, 73, 0.88)` (135deg)
- Flex layout: image left, text right (stacks on mobile)
- Line art max-height: 420px

## Future Considerations
- Additional tribute pages for other physicians affected by occupational radiation
- Integration with main ORSIF website navigation
- Potential Spanish translation (Juan was from Spain)

# YPO Austin Landing Page Plan

## 1. Objectives & Audience
- Communicate what YPO and YPO Austin are, highlighting exclusivity, warmth, and seriousness.
- Enable qualified CEOs/Presidents under 45 in Central Texas to self-qualify quickly.
- Encourage prospects to apply to YPO Austin first when evaluating YPO chapters.

## 2. Tech Stack & Structure
- Plain HTML5 + CSS3 (no build tooling required) for portability inside repo.
- Single-page layout with sticky navigation linking to anchored sections via smooth scrolling.
- Max content width 1180px with responsive padding (48px desktop, 24px mobile).

## 3. Section-by-Section Layout
1. **Hero (#hero)**
   - Full-height gradient background using --color-blue-dark → --color-blue.
   - Left column: eyebrow, H1, supporting copy, credibility pill, CTA buttons.
   - Right column: abstract geometric illustration block (CSS shapes) implying Austin skyline.
2. **About (#about)**
   - Two columns describing YPO global vs Austin chapter, stacked on mobile.
   - Badge highlighting “Top-performing chapter in the Western U.S. Region”.
3. **Members (#members)**
   - Intro text + 3x3 grid of stat cards with subtle drop shadow.
4. **Values (#values)**
   - Warm beige background, four value cards (2x2 desktop, stacked mobile).
5. **Criteria (#criteria)**
   - Side-by-side layout: descriptive copy + checklist styled with accent bullets.
   - CTA block with primary button + secondary text link.
6. **Process (#process)**
   - Five-step vertical timeline with numbered nodes and connecting line.
7. **Why YPO Austin (#why-austin)**
   - Dark blue band, four pillar cards with white copy.
8. **FAQ (#faq)**
   - Off-white background accordion; pure CSS details/summary for toggling.
9. **Footer (#footer)**
   - Dark background, two-column layout (about blurb + quick links/contact) plus bottom bar.

## 4. Navigation & Interactions
- Sticky header (64px) with semi-opaque surface, blur, and CTA button linking to #criteria.
- Mobile navigation: hamburger toggles dropdown overlay (CSS + checkbox hack) with same links.
- Smooth scrolling via `scroll-behavior: smooth` on `html`.
- Buttons styled per spec (pill primary gold, secondary text link).

## 5. Visual System
- CSS custom properties for palette provided in spec; reused across sections.
- Typography: Inter/system stack; font sizes per spec with responsive scaling using clamp().
- Cards: white surface, 14px radius, `box-shadow: 0 20px 50px rgba(0,0,0,0.04)`.
- Illustrative elements (hero shapes, dividers) use burnt orange + gold highlights.

## 6. Content Data Modeling
- Stats, values, criteria groups, process steps, pillars, FAQ stored as semantic HTML lists for easy future port to React props.

## 7. Responsiveness & Accessibility
- CSS Grid + Flexbox, breakpoints at 768px and 1024px.
- Focus states for interactive items; accessible nav labels.
- Buttons and links maintain sufficient color contrast (WCAG AA).

## 8. Future Enhancements (Optional)
- Replace hero illustration with optimized SVG skyline.
- Hook CTA buttons to external application form.
- Add analytics + form handling when backend available.

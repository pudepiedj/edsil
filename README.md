# EDSIL Website v3 - Complete Page Templates

All pages with dropdown header navigation. You just need to add your content.

## Files

```
index.html              - Home page (hero + MORE button)
mission.html            - Mission page
ride-ai.html            - RIDE⋮AI overview
ai-education.html       - AI and Education
programme.html          - The Programme
portfolio.html          - Portfolio overview
aga-khan-academy.html   - School detail page
uwc-dilijan.html        - School detail page
yiwu-academy.html       - School detail page
xuzhou-academy.html     - School detail page
judge-business-academy.html - School detail page
dragon-spruce.html      - School detail page
about.html              - About overview
john-puddefoot.html     - Bio page
susan-jesudason.html    - Bio page
contact.html            - Contact page
css/styles.css          - Stylesheet
```

## To Preview

```bash
cd edsil-v3-complete
python3 -m http.server 8000
```

## How to Add Content

1. Look for `<!-- YOUR CONTENT -->` placeholders
2. Replace with your content
3. For school pages: add image to `images/` folder
4. For bio pages: add photo to `images/` folder

## Page Types

**Standard content page** (mission, ride-ai, etc.):
```html
<section class="content-section">
  <h2>Section Title</h2>
  <p>Your paragraph text...</p>
</section>
```

**School detail page**:
- Has `school-content` layout with image + text side by side
- Has "Back to Portfolio" link

**Bio page**:
- Has `bio-layout` with photo + bio side by side
- Has "Back to About" link

## Images Needed

Create an `images/` folder and add:
- `john-puddefoot.jpg`
- `susan-jesudason.jpg`
- `aga-khan-academy.jpg`
- `uwc-dilijan.jpg`
- `yiwu-academy.jpg`
- `xuzhou-academy.jpg`
- `judge-business-academy.jpg`
- `dragon-spruce.jpg`

## Blog

Blog link points to `/blog/` - your existing Jekyll blog should work at that path.

## Deployment

Replace your existing site files with these, keeping your:
- `/blog/` folder (Jekyll)
- `images/` folder
- `CNAME` file

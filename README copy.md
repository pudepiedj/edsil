# EDSIL Website Additions

## Files Included

### HTML Pages
- `portfolio.html` - Updated portfolio with links to individual school pages
- `about.html` - Updated about page with full bios for John and Susan
- `aga-khan-academy.html` - Aga Khan Academy, Hyderabad detail page
- `uwc-dilijan.html` - UWC Dilijan detail page
- `judge-business-academy.html` - Judge Business Academy detail page
- `xuzhou-academy.html` - Xuzhou Academy detail page
- `yiwu-academy.html` - Yiwu Academy detail page
- `dragon-spruce.html` - Dragon Spruce BeeMee Schools detail page

### CSS
- `styles-additions.css` - Additional styles to append to your existing css/styles.css

## Installation Steps

1. **Copy HTML files** to your repo root (same level as index.html)

2. **Add CSS** - Append the contents of `styles-additions.css` to your existing `css/styles.css`

3. **Add images** - Create an `images/` folder and add:
   - `john-puddefoot.jpg` - John's photo
   - `susan-jesudason.jpg` - Susan's photo
   - `aga-khan-academy.jpg` - AKA Hyderabad photo
   - `uwc-dilijan.jpg` - UWC Dilijan photo
   - `judge-business-academy.jpg` - Judge Business Academy photo
   - `xuzhou-academy.jpg` - Xuzhou main photo
   - `xuzhou-1.jpg`, `xuzhou-2.jpg`, `xuzhou-3.jpg` - Xuzhou gallery (optional)
   - `yiwu-academy.jpg` - Yiwu photo
   - `dragon-spruce.jpg` - Dragon Spruce/BeeMee photo

4. **Commit and push**
   ```bash
   git add -A
   git commit -m "Add school detail pages and updated about page"
   git push
   ```

## Notes

- The school pages for Eton and S. Thomas' College don't have detail pages since they're historic positions (add if you want)
- Image paths assume images are in `/images/` folder - adjust if you use a different structure
- The gallery on Xuzhou page is optional - remove the `.school-gallery` div if not using
- Test locally before pushing: `python -m http.server 8000` then visit localhost:8000

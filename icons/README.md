# Extension Icons

Place PNG icons here with these sizes:

- `icon16.png` - 16x16 pixels (toolbar)
- `icon32.png` - 32x32 pixels (Windows)
- `icon48.png` - 48x48 pixels (extensions page)
- `icon128.png` - 128x128 pixels (Chrome Web Store)

## Quick Generation

You can generate simple icons using ImageMagick:

```bash
# Create a simple colored square icon
convert -size 128x128 xc:'#1a1a1a' -fill white -gravity center -pointsize 80 -annotate 0 'F' icon128.png
convert icon128.png -resize 48x48 icon48.png
convert icon128.png -resize 32x32 icon32.png
convert icon128.png -resize 16x16 icon16.png
```

Or use an online tool like:
- https://favicon.io/
- https://www.canva.com/

## Design Guidelines

- Simple, recognizable shape
- Works on light and dark backgrounds
- Avoid text (too small to read at 16px)

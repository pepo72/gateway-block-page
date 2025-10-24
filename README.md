# Gateway Block Page

Custom pixel-art styled block page for Cloudflare Zero Trust Gateway.

## Features

- Retro CRT terminal aesthetic
- ASCII art skull graphic
- Scanline and glitch effects
- Dynamic Cloudflare Gateway variables
- Responsive design

## Deployment

### GitHub Pages

1. Enable GitHub Pages in repository settings
2. Source: main branch
3. URL will be: `https://pepo72.github.io/gateway-block-page/`

### Cloudflare Gateway Setup

1. Go to Zero Trust > Settings > Custom Pages
2. Select "Account Gateway block page"
3. Choose "URL redirect"
4. Enter: `https://pepo72.github.io/gateway-block-page/`
5. Save

## Variables

The page uses these Cloudflare Gateway variables:

- `{{BLOCKED_URL}}` - The blocked destination
- `{{BLOCK_REASON}}` - Reason for blocking
- `{{CATEGORY}}` - Block category
- `{{BLOCK_ID}}` - Unique block identifier

## Customization

Edit `index.html` to modify:
- Colors (currently green terminal theme)
- Text content
- ASCII art
- Layout

## License

MIT

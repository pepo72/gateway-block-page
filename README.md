# Gateway Block Page

Custom cyberpunk-styled block page for Cloudflare Zero Trust Gateway.

![Preview](https://img.shields.io/badge/style-cyberpunk-00ff41?style=flat-square)

## Features

- 🖥️ CRT terminal aesthetic with scanlines and vignette
- 💀 ASCII art "BLOCK" banner
- ⚡ Glitch animation on title
- 📟 Typewriter terminal animation
- 🔲 Animated background grid
- 📊 Status bar with threat indicator
- 📱 Fully responsive (mobile-friendly)
- 🎨 Cyberpunk color scheme (green/amber/red)
- 🔗 Dynamic Cloudflare Gateway variables

## Preview

The page features:
- Animated grid background with scrolling effect
- CRT-style scanlines overlay + vignette darkening
- "BLOCK" ASCII art in red with glow
- Status bar showing threat detection
- Terminal-style log with typewriter animation
- Blocked URL highlighted in amber
- Reason/Category in a clean card grid
- Gradient divider and minimal footer

## Cloudflare Gateway Variables

| Variable | Description |
|----------|-------------|
| `{{BLOCKED_URL}}` | The blocked destination URL |
| `{{BLOCK_REASON}}` | Reason for blocking |
| `{{CATEGORY}}` | Block category |
| `{{BLOCK_ID}}` | Unique incident identifier |

## Deployment

### GitHub Pages

1. Enable GitHub Pages in repository settings
2. Source: main branch, root `/`
3. URL: `https://pepo72.github.io/gateway-block-page/`

### Cloudflare Gateway Setup

1. Go to **Zero Trust → Settings → Custom Pages**
2. Select **Account Gateway block page**
3. Choose **URL redirect**
4. Enter: `https://pepo72.github.io/gateway-block-page/`
5. Save

## Customization

All styling is in a single `index.html` file. Key CSS variables:

```css
:root {
    --green: #00ff41;    /* Primary terminal color */
    --red: #ff0040;      /* Warning/threat color */
    --amber: #ffb000;    /* URL/highlight color */
    --bg: #0a0a1a;       /* Background */
}
```

## License

MIT

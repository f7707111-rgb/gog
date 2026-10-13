# kiki — Graphic Designer portfolio

Static site. No build step: extract the folder and open `index.html`, or deploy the complete folder to your host.

## Current home page

- Game Boy hero with a generated pixel-art idea meadow and a crisp pixel dissolve into the normal page background; EN/RU language switch.
- Animated poster workspace with a demonstration conversation.
- Telegram and mail banners.
- GitHub and Community banners with translucent glass backing in the style of the folder pockets.
- Five folder chapters: about, works, services, process, contact.
- Pixel-art footer with cursor-following tilt, image parallax and light.

The site uses the original light background through the very bottom. Theme switching, the Toolkit button/modal and the software folder have been removed.

## Files

- `index.html`: home page.
- `section.html?s=about|works|services|process|contact`: chapter pages.
- `js/data/translations.js`: EN/RU UI copy.
- `js/data/sections.js`: folder definitions and chapter content.
- `css/components/community-glass.css`: glass backing for GitHub/Community.
- `css/components/design-studio.css`, `js/site/design-studio.js`: animated design demo.
- `css/components/portfolio-footer.css`, `js/site/portfolio-footer.js`: footer and cursor motion.
- `assets/images/footer-pixel-art.webp`: generated footer artwork.

Mouse/pen motion responds to real pointer events and works with a mouse on touch-capable computers. Touch gestures are not hijacked. Reduced-motion preferences are respected. PNG previews are static; test movement in the actual HTML page.

## Pixel hero wallpaper

`assets/images/hero-meadow-transition.webp` contains the idea-meadow artwork and its square-pixel transparent bottom edge in ONE image. No separate mask image is needed. `css/components/hero-pixel.css?v=2` positions the background at the bottom so cover-cropping cannot remove the transition. The unchanged `--site-bg` shows through the transparent pixels.

The standalone “From your idea to a design that’s ready to go” banner is removed. The original poster/chat banner and the How I work folder are kept.

When deploying, upload the complete updated folder, including the new artwork and stylesheet; replacing the background image alone will not apply the CSS change.

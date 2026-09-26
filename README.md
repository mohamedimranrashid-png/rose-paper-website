# Rose Paper website

A static website (plain HTML, no build step) for Rose Paper Stationery and Gifts Sdn. Bhd.

## What's in here
- `index.html`: the whole site
- `img/`: banner and category photos
- `favicon.svg`, `apple-touch-icon.png`: browser-tab and phone icons
- `og-image.png`: the preview picture WhatsApp and Facebook show when the link is shared
- `netlify.toml`: Netlify settings (publish this folder, cache the images)

## Put it live on Netlify
1. Go to Netlify and choose **Add new site → Import an existing project → GitHub**, then pick this repository.
2. Leave the build command empty and set the publish directory to `.`.
3. Deploy. Every change pushed to GitHub goes live automatically.

## After you connect a domain
Change `og:image` in `index.html` to the full address, for example `https://yourdomain.com.my/og-image.png`. WhatsApp link previews need a full address.

## Adding product photos
Each product in `index.html` (search for `var P=[`) can take an `img` field, for example `img:'img/products/a4-80.jpg'`. Put the photo in `img/products/`, square format, on a coloured background.

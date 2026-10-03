# Save the Capybara!

A colourful browser game for kids. A storm has blown the capybaras into the clouds, and you catch them on your lily pad as they float down on leaf parachutes.

- 15 levels across five worlds: Sunny Skies, Windy Day, Starry Night, Autumn Leaves and Holiday Snow
- Easy, Medium and Hard modes, each with its own stars
- A Capy Club of friends to unlock, party music and sound effects
- Works on phones, tablets and computers (touch, mouse or arrow keys)

The whole game is one file, `index.html`, with no build step. Progress is saved in the player's browser only.

## Publishing

The site is hosted with GitHub Pages from the `main` branch and the repository root (`/`).

Custom domain:

- `https://savethecapybara.com`

Cloudflare is used for DNS management and Web Analytics. The DNS records point the domain to GitHub Pages, while analytics is added manually in `index.html` using the Cloudflare Web Analytics JavaScript snippet.

### GitHub Pages settings

In the repository:

- Go to **Settings → Pages**
- Source: **Deploy from a branch**
- Branch: **main**
- Folder: **/(root)**
- Custom domain: **savethecapybara.com**
- **Enforce HTTPS**: enabled

### Cloudflare DNS

The domain uses GitHub Pages records:

- `A` → `185.199.108.153`
- `A` → `185.199.109.153`
- `A` → `185.199.110.153`
- `A` → `185.199.111.153`
- `CNAME` for `www` → `jamierafferty15.github.io`

The DNS records are left as **DNS only** rather than proxied.

### Cloudflare Web Analytics

Cloudflare Web Analytics is installed manually in `index.html` using the JavaScript beacon snippet provided by Cloudflare.

The analytics snippet should be placed immediately before the closing `</body>` tag.

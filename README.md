# Uncarriable

An art collective. Undefined, uncontainable.

## Stack

- **Three.js** (r163) — WebGL 3D scene with instanced geometry
- **UnrealBloomPass** — post-processing glow via Three.js addons
- **Vanilla HTML/CSS/JS** — single self-contained `index.html`, no build step

## Local development

Open `index.html` in any modern browser. That's it.

For hot-reload during development, serve the directory:

```bash
npx http-server . -p 3000 -c-1
```

Then open `http://localhost:3000`.

## Deploy on GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Under **Source**, select **Deploy from a branch**
4. Set branch to `main`, folder to `/ (root)`
5. Save — the site will be live at `https://<username>.github.io/uncarriable/`

### Custom domain (uncarriable.com via Squarespace DNS)

In **Squarespace Domains → DNS Settings**, add these records:

| Type  | Host | Value                       |
|-------|------|-----------------------------|
| A     | @    | 185.199.108.153             |
| A     | @    | 185.199.109.153             |
| A     | @    | 185.199.110.153             |
| A     | @    | 185.199.111.153             |
| CNAME | www  | n-q-m-e.github.io          |

Then in **GitHub repo → Settings → Pages → Custom domain**, enter `uncarriable.com` and enable **Enforce HTTPS**.

DNS propagation can take up to 24–48 hours.

## Customizing the color cycle

In `index.html`, find the `COLORS` array near the top of the `<script>` block:

```js
const COLORS = [
  new THREE.Color('#0040ff'), // electric blue
  new THREE.Color('#ff4400'), // volcanic orange
  new THREE.Color('#8800ff'), // dense violet
  new THREE.Color('#cc0033')  // deep ruby
];
const CYCLE_DURATION = 270; // seconds for a full cycle (~4.5 min)
```

- Change hex values to use different colors
- Add or remove entries to change the number of color stops
- Adjust `CYCLE_DURATION` (in seconds) to speed up or slow down transitions

## License

All rights reserved.

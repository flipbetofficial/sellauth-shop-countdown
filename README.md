# Shop Sell Auth

Premium digital products marketplace — Discord, Robux, and social media growth services.

## Tech Stack

- React 19 + TypeScript
- Vite 7
- Tailwind CSS v4
- Framer Motion
- shadcn/ui components (Radix UI)
- Sonner toasts
- localStorage for order persistence

## Local Development

```bash
npm install
npm run dev
```

Open http://localhost:5173

## Build

```bash
npm run build
```

Output goes to `dist/`.

---

## Deploy to Cloudflare Pages (via GitHub)

1. Push this repo to GitHub.
2. Go to [Cloudflare Pages](https://pages.cloudflare.com/) → **Create a project** → **Connect to Git**.
3. Select your repository.
4. Set the following build settings:

| Setting | Value |
|---|---|
| **Framework preset** | None (or Vite) |
| **Build command** | `npm run build` |
| **Build output directory** | `dist` |
| **Node.js version** | 18 or higher |

5. Click **Save and Deploy**.

That's it — Cloudflare Pages will build and deploy automatically on every push to `main`.

---

## Customisation

| What | Where |
|---|---|
| Products & prices | `src/lib/constants.ts` |
| LTC wallet address | `src/pages/store.tsx` — search `LTC_ADDRESS` |
| Discord link | `src/pages/store.tsx` — search `discord.gg` |
| Colours / theme | `src/index.css` — CSS variables under `:root` |
| Store name / tagline | `src/pages/store.tsx` + `index.html` |

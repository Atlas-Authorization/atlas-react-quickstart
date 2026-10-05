# atlas-react-quickstart

A minimal Vite + React app pre-wired with [Atlas](https://atlasauth.net) auth,
using `@atlasauth/react`.

## What it shows

- `src/main.tsx` — the app wrapped in `<AtlasProvider>`, configured from your
  `VITE_ATLAS_*` environment variables.
- `src/App.tsx` — `<SignedOut>` renders the `<SignIn>` flow; `<SignedIn>` shows
  the current user (via `useUser`) and a `<UserButton>`.

## Run it

1. `npm install`
2. `cp .env.example .env`, then set `VITE_ATLAS_PUBLISHABLE_KEY` (and adjust
   `VITE_ATLAS_FRONTEND_API`) to the values from
   [atlasauth.net](https://atlasauth.net).
3. `npm run dev`

Open the URL Vite prints (defaults to http://localhost:5173).

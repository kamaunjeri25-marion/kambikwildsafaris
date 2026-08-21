# Aura Stay Dine

A luxury travel and dining discovery app built with React, Vite, TypeScript, Tailwind CSS, and shadcn/ui. The experience combines a premium landing page, curated discovery flows, AI concierge chat, and Supabase-powered authentication.

## Features

- Premium hospitality landing page
- Hotel and restaurant discovery experience
- AI concierge chat for trip recommendations
- Supabase authentication for sign in and sign up
- PWA install prompt support
- Responsive design tailored for mobile and desktop

## Tech Stack

- Vite
- React 18
- TypeScript
- Tailwind CSS
- shadcn/ui
- Supabase
- React Router
- TanStack Query

## Local Development

1. Install dependencies:

```bash
npm install
```

2. Create a local environment file:

```bash
cp .env.example .env
```

3. Add your project values to `.env`:

```bash
VITE_SUPABASE_URL="https://your-project-id.supabase.co"
VITE_SUPABASE_PUBLISHABLE_KEY="your-anon-key"
```

4. Start the Vite app:

```bash
npm run dev
```

5. Open the local URL shown in the terminal.

## Production Build

```bash
npm run build
```

## Environment Notes

This project expects Supabase to be configured for:

- authentication flows in the auth pages
- AI chat function calls through the Supabase Edge function
- optional future data-backed booking or profile features

For the AI chat integration, ensure the Supabase function has access to the required environment secret for the AI gateway.

## Project Structure

```text
src/
  App.tsx
  main.tsx
  pages/
    Index.tsx
    Discover.tsx
    Auth.tsx
    AIChat.tsx
  components/
  hooks/
  integrations/
    supabase/
      client.ts
supabase/
  functions/
    ai-chat/
      index.ts
```

## Scripts

- `npm run dev` — run the app locally
- `npm run build` — build a production bundle
- `npm run preview` — preview the built app
- `npm run lint` — run ESLint checks

## License

This project is for demo and portfolio use unless otherwise specified by the repository owner.

# PDF Maker

A web app that turns scanned documents and images into clean, downloadable PDFs — with AI-assisted processing.

Live demo: [pdf-maker-pink.vercel.app](https://pdf-maker-pink.vercel.app)

## What it does

- Scan or upload documents and images
- AI-assisted processing for cleaner output
- Generate and download PDFs client-side
- Secure backend with authentication and storage

## Tech stack

- **Frontend:** React 18, TypeScript, Vite, Tailwind CSS, shadcn/ui
- **PDF generation:** jsPDF (client-side)
- **AI:** Google Generative AI SDK
- **Backend:** Supabase (auth, database, storage)
- **Forms:** React Hook Form + Zod
- **Deployment:** Vercel

## Getting started

```bash
# Install dependencies
npm install

# Set up environment variables
# Create a .env file with your Supabase and Google AI credentials:
# VITE_SUPABASE_URL=your-supabase-url
# VITE_SUPABASE_ANON_KEY=your-supabase-anon-key
# VITE_GOOGLE_AI_API_KEY=your-google-ai-key

# Run the dev server
npm run dev
```

## Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm run lint` | Run ESLint |

## Project structure

```
src/
├── components/     # UI components (shadcn/ui based)
├── pages/          # Routes (Index, NotFound)
├── hooks/          # Custom React hooks
├── integrations/   # Supabase client setup
├── lib/            # Utilities
└── types/          # TypeScript types
supabase/           # Supabase migrations/config
```

## License

MIT

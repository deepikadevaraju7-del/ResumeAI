# ResumeAI

ResumeAI screens resumes against a job description and surfaces structured skills, experience, and match signals for recruiter review.

## Local development

Requires Node.js 20 or newer.

```sh
git clone https://github.com/deepikadevaraju7-del/ResumeAI.git
cd ResumeAI
npm install
npm run dev
```

The development server is available at `http://localhost:8080`.

## Environment variables

Create a local `.env` file, or add these variables in the Vercel project settings:

```env
VITE_SUPABASE_URL=
VITE_SUPABASE_PUBLISHABLE_KEY=
SUPABASE_URL=
SUPABASE_PUBLISHABLE_KEY=
SUPABASE_SERVICE_ROLE_KEY=
LOVABLE_API_KEY=
```

The `VITE_` variables are exposed to the browser. Keep `SUPABASE_SERVICE_ROLE_KEY` and `LOVABLE_API_KEY` server-only.

## Validation

```sh
npm run lint
npm run build
```

The production build uses Nitro's Vercel preset and emits the Vercel Build Output API directory automatically.

## Deploy to Vercel

Import `https://github.com/deepikadevaraju7-del/ResumeAI` into Vercel. Vercel will use the repository's `npm run build` command and the generated Nitro server function. Add the environment variables above for Preview and Production environments before deploying.

# APIForge — API testing workspace

A responsive API request workspace built with React, Vite, Framer Motion and Lucide icons. Includes request composition, query parameters, headers, JSON body editing, browser fetch execution, response inspection, request history, collections, environment variables, cURL generation, and workspace import/export.

## Run locally

1. Install Node.js 18 or newer.
2. In this folder, run `npm install`.
3. Run `npm run dev` and open the local URL printed by Vite.
4. Run `npm run build` to create the production build in `dist/`.

## Deploy to Vercel

Import the GitHub repository into Vercel. Vercel should detect Vite automatically. Use:
- Framework preset: Vite
- Build command: `npm run build`
- Output directory: `dist`
- Install command: `npm install`

No environment variables are required for the included features.

## Included features

- GET, POST, PUT, PATCH, DELETE, HEAD and OPTIONS requests
- Editable query parameters and headers
- Request body editor
- Response status, duration, size, body and headers
- Local request history and collections
- Environment variables using `{{variable_name}}` syntax
- cURL command generation
- JSON workspace import/export
- Local browser persistence using `localStorage`
- Curiosity Labs logo animation and attribution footer

## Important limitations

Requests are sent directly from the browser using `fetch`. Some APIs reject browser-originated requests because of CORS policy. This is a browser security restriction, not an APIForge bug. For those APIs, add a trusted server-side proxy/backend before production use. Data is stored in the current browser profile; this starter does not include accounts, cloud sync, team sharing, or a server database. Never store production secrets in a browser environment.

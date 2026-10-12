# HouseHunt Frontend
React frontend for the HouseHunt rental management capstone.

Live website: https://househunt-production-6767.up.railway.app
Backend code: https://github.com/Spoorthy2815/househunt-backend

## Technologies and features
React, Vite, React Router, Axios, Bootstrap, custom responsive CSS, Lucide React, React Markdown, Vitest and React Testing Library.
Includes search/filtering, property details, registration/login, protected pages, owner dashboards, admin review, bookings, saved homes, preferences and assistant chat.

## Run locally
Requires Node.js 22.12+ or 24 and the backend on port 8080.
npm ci
npm run dev

Open http://localhost:5173. Vite proxies /api to http://localhost:8080. Port 5173 is strict.

## Verify
npm test
npm run build

For independent hosting, set VITE_API_URL to the backend HTTPS /api URL before building, and set backend CORS_ORIGIN to the frontend origin. Configure SPA rewrites to index.html. VITE_ variables are public; never place secrets in them.

## Source
src/main.jsx: app routing
src/ui.jsx: authentication and shared components
src/pages/: page components
src/api.js: Axios client and interceptors
src/styles.css: responsive CSS

The Dockerfile/nginx.conf expects a backend service named backend on the same Docker network.
The existing live deployment remains connected to https://github.com/Spoorthy2815/househunt-capstone. This separate repository is for coursework review and independent development; pushing here does not update the live app automatically.
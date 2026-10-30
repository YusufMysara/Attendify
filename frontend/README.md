# Attendify web app

The browser client for Attendify, built with React, TypeScript and Vite. Admins manage users, courses, enrollments and student photos; teachers run live attendance sessions with the camera, review and submit them, and see reports. Students can also log in to see their attendance history and stats.

The frontend was started from a Lovable template; I built the backend.

## Stack

React 18 · TypeScript · Vite · Tailwind CSS · shadcn/ui · TanStack Query · React Router

## Run it

You need Node.js 18+ and the backend running (see the main README).

```bash
cd frontend
npm install
```

Create `frontend/.env` with the backend address:

```env
VITE_API_BASE_URL=http://localhost:8000
```

Start the dev server, then open <http://localhost:8080>:

```bash
npm run dev
```

Other scripts: `npm run build` (production build in `dist/`), `npm run preview` (serve the build), `npm run lint`.

## Structure

```
src/
  pages/admin/     users, courses, photo upload, attendance records
  pages/teacher/   courses, live camera, session review, reports
  pages/student/   dashboard, attendance history, stats
  components/      shared UI
```

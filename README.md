# React Admin Dashboard

A responsive admin dashboard UI built with React, TypeScript and Vite. It includes a dashboard with charts, data tables for users and products, and detail pages. All data is mocked on the client.

## Features

- Dashboard with stat cards, line, bar, area and pie charts
- Users and products pages with a sortable, filterable, paginated data table
- "Add" modal with a form generated from the table columns
- Detail pages for a single user and a single product
- Sidebar navigation, top bar and footer layout
- Client-side routing with React Router
- Responsive layout built with SCSS

## Tech stack

- React 18
- TypeScript
- Vite
- React Router
- MUI X Data Grid
- Recharts
- TanStack Query
- Sass

## Getting started

Requirements: Node.js 18 or newer.

```bash
git clone https://github.com/<your-username>/react-admin-dashboard.git
cd react-admin-dashboard
npm install
npm run dev
```

The app will be available at `http://localhost:5173`.

## Scripts

| Command           | Description                          |
| ----------------- | ------------------------------------ |
| `npm run dev`     | Start the development server         |
| `npm run build`   | Type-check and build for production  |
| `npm run preview` | Preview the production build locally |

## Project structure

```
src/
  components/   Reusable UI pieces (navbar, menu, charts, data table, ...)
  pages/        Route-level pages (home, users, products, user, product, login)
  styles/       Global styles, variables and responsive mixins
  data.ts       Mock data used across the app
  App.tsx       Layout and routes
```

## Notes

- All data comes from `src/data.ts`. Creating and deleting records is not persisted yet.
- TanStack Query is configured and ready to be used once a real API is connected.
- The login page is a placeholder.

## Roadmap

- Connect a REST API with a database
- Implement authentication and role-based access
- Wire up create, update and delete actions
- Add form validation

## License

MIT

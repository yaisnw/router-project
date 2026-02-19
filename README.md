# Pet Adoption App

> A pet adoption website built with React Router v6 — browse pets by type, search, and view detailed profiles. Created in December 2023 as a Codecademy guided project, recently updated for GitHub Pages deployment.

🔗 **[Live Demo](https://yaisnw.github.io/router-project)**

---

## Features

- 🐶 **Browse by pet type** — dogs, cats, rabbits, birds
- 🔍 **Search** by name or location
- 📄 **Pet detail pages** with breed, color, gender, and description
- 🧭 **Active navigation** highlights current pet type
- 🚫 **404 handling** for missing pet details

---

## Recent Updates

Coming back to this project in 2026 to deploy on GitHub Pages, I fixed several routing and path issues:

- **Added `basename`** to `createBrowserRouter` to handle the `/router-project` subpath correctly
- **Fixed static asset URLs** — CSS and images now use correct relative paths (`%PUBLIC_URL%`) instead of absolute paths
- **Configured MSW service worker** to register at the correct scope for GitHub Pages deployment

---

## Tech Stack

| Technology | Purpose |
|---|---|
| React 18 | UI framework |
| React Router v6 | Client-side routing |
| MSW (Mock Service Worker) | Mock API for pet data |
| Create React App | Build tool |
| GitHub Pages | Hosting |

---

## React Router Concepts Demonstrated

- `createBrowserRouter` with `basename` for GitHub Pages
- `NavLink` with active state styling
- `useParams` for dynamic route parameters
- `useNavigate` for programmatic navigation
- `useSearchParams` for query string handling
- `Navigate` component for redirects
- `Outlet` for nested route rendering
- `Link` component for declarative navigation

---

## Getting Started

### Prerequisites
- Node.js 20+

### Installation

```bash
git clone https://github.com/yaisnw/router-project.git
cd router-project
npm install
```

### Running Locally

```bash
npm start
```

The app uses Mock Service Worker to simulate an API — pet data is stored in `/src/mocks/data/`.

### Deployment

```bash
npm run deploy
```

---

## Notes

This was a guided Codecademy project focused on learning React Router v6. The pet data is mocked using MSW, and some external pet images from the original mock data may not load due to expired CDN URLs.

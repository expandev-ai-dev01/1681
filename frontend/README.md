# AutoClean Frontend

A React-based frontend application for the AutoClean file cleanup tool.

## Features

- Identify and remove temporary files
- Detect duplicate files
- Free up disk space automatically

## Tech Stack

- React 19.2.0
- TypeScript 5.6.3
- Vite 5.4.11
- TailwindCSS 3.4.14
- React Router 7.9.3
- TanStack Query 5.90.2
- Axios 1.12.2
- Zustand 5.0.8

## Getting Started

### Prerequisites

- Node.js 18+ and npm

### Installation

```bash
npm install
```

### Environment Setup

Copy `.env.example` to `.env` and configure:

```bash
cp .env.example .env
```

### Development

```bash
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

### Build

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

## Project Structure

```
src/
├── app/                 # Application configuration
│   ├── App.tsx         # Root component
│   └── router.tsx      # Routing configuration
├── assets/             # Static assets
│   └── styles/         # Global styles
├── core/               # Core utilities and components
│   ├── components/     # Shared components
│   ├── lib/           # Library configurations
│   └── utils/         # Utility functions
├── domain/            # Business domains
├── pages/             # Page components
│   ├── layouts/       # Layout components
│   ├── Home/          # Home page
│   └── NotFound/      # 404 page
└── main.tsx           # Application entry point
```

## API Configuration

The application connects to the backend API using environment variables:

- `VITE_API_URL`: Backend API base URL (default: http://localhost:3000)
- `VITE_API_VERSION`: API version (default: v1)
- `VITE_API_TIMEOUT`: Request timeout in milliseconds (default: 30000)

## License

MIT
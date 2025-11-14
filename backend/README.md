# AutoClean Backend

Backend API for AutoClean - File management and cleanup system.

## Description

Simple script that identifies and removes temporary or duplicate files from a folder.

## Features

- Identify and remove temporary files
- Detect common temporary file extensions (.tmp, .temp, .cache)
- System temporary file pattern recognition
- Automatic disk space cleanup

## Technology Stack

- **Runtime**: Node.js
- **Language**: TypeScript
- **Framework**: Express.js
- **Database**: MS SQL Server
- **Architecture**: REST API

## Project Structure

```
src/
├── api/                    # API controllers
│   └── v1/                 # API version 1
│       ├── external/       # Public endpoints
│       └── internal/       # Authenticated endpoints
├── routes/                 # Route definitions
│   └── v1/                 # Version 1 routes
├── middleware/             # Express middleware
├── services/               # Business logic
├── utils/                  # Utility functions
├── constants/              # Application constants
├── instances/              # Service instances
├── config/                 # Configuration
├── tests/                  # Global test utilities
└── server.ts               # Application entry point
```

## Getting Started

### Prerequisites

- Node.js 18+
- MS SQL Server
- npm or yarn

### Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```

3. Copy `.env.example` to `.env` and configure:
   ```bash
   cp .env.example .env
   ```

4. Update `.env` with your database credentials

### Development

Run the development server:
```bash
npm run dev
```

The API will be available at `http://localhost:3000`

### Building

Build for production:
```bash
npm run build
```

### Running Production

Start the production server:
```bash
npm start
```

## API Documentation

### Health Check

```
GET /health
```

Returns the health status of the API.

### API Versioning

All API endpoints are versioned:
- Version 1: `/api/v1/`

## Testing

Run tests:
```bash
npm test
```

Run tests in watch mode:
```bash
npm run test:watch
```

## Code Quality

Lint code:
```bash
npm run lint
```

Fix linting issues:
```bash
npm run lint:fix
```

## Environment Variables

See `.env.example` for all available configuration options.

## License

ISC
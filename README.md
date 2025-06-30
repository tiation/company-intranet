# Company Intranet

A modern company intranet application built with Vue 3, TypeScript, and Tailwind CSS.

## Tech Stack

- **Vue 3** - Progressive JavaScript framework
- **TypeScript** - Type-safe JavaScript
- **Vite** - Fast build tool and dev server
- **Vue Router** - Official router for Vue.js
- **Pinia** - Vue state management
- **Tailwind CSS** - Utility-first CSS framework
- **ESLint** - Code linting
- **Prettier** - Code formatting

## Project Structure

```
src/
├── components/      # Reusable UI components
├── views/          # Page components
├── stores/         # Pinia stores for state management
├── router/         # Vue Router configuration
├── services/       # API services and external integrations
├── types/          # TypeScript type definitions
├── composables/    # Vue composables (reusable logic)
└── assets/         # Static assets
```

## Environment Variables

Copy `.env.example` to `.env` and configure:

```bash
VITE_API_BASE_URL=http://localhost:3000/api
VITE_APP_NAME=Company Intranet
VITE_APP_VERSION=1.0.0
```

## Development

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Type checking
npm run type-check

# Linting
npm run lint

# Code formatting
npm run format
```

## Production

```bash
# Build for production
npm run build

# Preview production build
npm run preview
```

## Features

- 📱 Responsive design with Tailwind CSS
- 🔧 TypeScript for type safety
- 🎨 Component-based architecture
- 🗂️ Organized folder structure
- 🔀 Vue Router for navigation
- 📊 Pinia for state management
- 🛠️ ESLint + Prettier for code quality
- ⚡ Vite for fast development

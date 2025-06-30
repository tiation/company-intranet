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

## GitHub Pages Deployment

This project is configured for automatic deployment to GitHub Pages using GitHub Actions.

### Setup Instructions

1. **Enable GitHub Pages in Repository Settings:**
   - Go to your repository on GitHub
   - Navigate to `Settings` → `Pages`
   - Under "Source", select `GitHub Actions`
   - Save the settings

2. **Automatic Deployment:**
   - Every push to the `main` branch will trigger a deployment
   - The GitHub Actions workflow will:
     - Install dependencies
     - Build the project
     - Deploy to GitHub Pages
   - Check the "Actions" tab to monitor deployment status

3. **Access Your Site:**
   - Once deployed, your site will be available at:
   - `https://tiation.github.io/company-intranet/`

### Manual Deployment

If you need to deploy manually:

```bash
# Build the project
npm run build

# The dist/ folder contains the built files ready for deployment
```

### Configuration Notes

- The `vite.config.ts` is configured with `base: '/company-intranet/'` for GitHub Pages
- The GitHub Actions workflow uses Node.js 18 and deploys the `dist` folder
- The workflow requires `pages: write` and `id-token: write` permissions

## Features

- 📱 Responsive design with Tailwind CSS
- 🔧 TypeScript for type safety
- 🎨 Component-based architecture
- 🗂️ Organized folder structure
- 🔀 Vue Router for navigation
- 📊 Pinia for state management
- 🛠️ ESLint + Prettier for code quality
- ⚡ Vite for fast development

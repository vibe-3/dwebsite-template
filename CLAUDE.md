# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

- `npm run dev` - Start development server at http://localhost:3000
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint

## Architecture

This is a Next.js 16 project using the App Router with TypeScript, Tailwind CSS v4, and React 19.

### Key Files

- `app/layout.tsx` - Root layout with Geist font configuration
- `app/page.tsx` - Home page component
- `app/globals.css` - Global styles with Tailwind v4 `@import "tailwindcss"` and CSS custom properties for theming

### Styling

- Uses Tailwind CSS v4 with PostCSS (`@tailwindcss/postcss`)
- Theme colors defined as CSS custom properties in `globals.css` (`--background`, `--foreground`)
- Dark mode supported via `prefers-color-scheme` media query
- Geist font family loaded via `next/font/google`

### Path Aliases

`@/*` maps to the project root (configured in `tsconfig.json`)

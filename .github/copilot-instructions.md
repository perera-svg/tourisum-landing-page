# Project Instructions

## Architecture & Structure

- **Framework**: Next.js 16 (App Router) with TypeScript.
- **Styling**: Tailwind CSS v4.
- **Directory Structure**:
  - `src/app/`: App Router pages, layouts, and route handlers.
  - `src/components/`: Reusable UI components (create if missing).
  - `src/lib/`: Utility functions and shared logic (create if missing).
- **Import Alias**: Use `@/*` to resolve paths from `./src/*`.

## Development Workflow

- **Package Manager**: `pnpm`.
- **Commands**:
  - Dev Server: `pnpm dev`
  - Build: `pnpm build`
  - Lint: `pnpm lint`

## Coding Conventions

- **Components**:
  - Default to **Server Components**. Use `"use client"` directive only when necessary (state, effects, event listeners).
  - Use functional components with named exports.
  - Place components in `src/components`.
- **Styling**:
  - Use Tailwind CSS utility classes.
  - Tailwind v4 configuration is in `src/app/globals.css` using CSS variables.
  - Use `clsx` or `tailwind-merge` for conditional class names if needed.
- **TypeScript**:
  - Use strict typing. Avoid `any`.
  - Define interfaces/types for component props.

## Key Files

- `src/app/layout.tsx`: Root layout, font configuration (Geist).
- `src/app/globals.css`: Global styles and Tailwind v4 theme configuration.
- `tsconfig.json`: TypeScript configuration and path aliases.

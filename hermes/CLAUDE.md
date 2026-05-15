# Hermès — AI Context for Claude

> This file provides context for Claude AI to assist with this React + TypeScript + Vite project.

---

## Project Overview

**Hermès** is a minimal React application scaffolded with Vite and TypeScript. It serves as a clean starting point for building modern web applications with fast HMR (Hot Module Replacement) and type safety.

---

## Tech Stack

- **React 18.3+** — UI library
- **TypeScript 5.5+** — Type-safe JavaScript
- **Vite 5.3+** — Build tool and dev server
- **ESLint** — Code linting
- **CSS** — Styling (no framework)

---

## Project Structure

```
hermes/
├── src/
│   ├── main.tsx          # Application entry point
│   ├── App.tsx           # Root component
│   ├── App.css           # Component styles
│   ├── index.css         # Global styles
│   └── vite-env.d.ts     # Vite type definitions
├── public/               # Static assets
├── index.html            # HTML template
├── vite.config.ts        # Vite configuration
├── tsconfig.json         # TypeScript config (app)
├── tsconfig.node.json    # TypeScript config (build tools)
└── package.json          # Dependencies and scripts
```

---

## Development Commands

```bash
# Install dependencies
npm install

# Start dev server (http://localhost:5173)
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview

# Lint code
npm run lint
```

---

## Code Conventions

### TypeScript
- Use `.tsx` for React components
- Use `.ts` for utilities and non-React code
- Enable strict mode (already configured)
- Prefer type inference over explicit types when obvious

### React
- Use functional components with hooks
- Use `React.FC` sparingly (prefer explicit return types)
- Keep components small and focused
- Extract reusable logic into custom hooks

### Styling
- Use CSS modules for component-specific styles
- Keep global styles minimal (in `index.css`)
- Use semantic class names
- Prefer CSS variables for theming

### File Organization
- One component per file
- Co-locate related files (component + styles + tests)
- Use `index.ts` for clean exports
- Keep `src/` flat until complexity requires folders

---

## AI Assistance Guidelines

When helping with this project:

1. **Respect the Stack**: Don't suggest adding routing, state management, or UI libraries unless explicitly requested
2. **Keep It Simple**: This is a minimal template — avoid over-engineering
3. **Type Safety**: Always provide proper TypeScript types
4. **Modern React**: Use hooks, not class components
5. **Vite-First**: Leverage Vite features (HMR, env variables, etc.)
6. **ESM Only**: Use ES modules syntax (`import`/`export`)

---

## Common Tasks

### Adding a New Component
```tsx
// src/components/Button.tsx
interface ButtonProps {
  label: string;
  onClick: () => void;
}

export function Button({ label, onClick }: ButtonProps) {
  return <button onClick={onClick}>{label}</button>;
}
```

### Using Environment Variables
```typescript
// Access Vite env variables
const apiUrl = import.meta.env.VITE_API_URL;
```

### Adding a Dependency
```bash
npm install <package-name>
npm install -D <dev-package-name>
```

---

## Troubleshooting

### Port Already in Use
```bash
# Vite will auto-increment port (5174, 5175, etc.)
# Or specify a port:
npm run dev -- --port 3000
```

### TypeScript Errors
```bash
# Clear cache and rebuild
rm -rf node_modules dist
npm install
npm run build
```

### HMR Not Working
- Check browser console for errors
- Restart dev server
- Clear browser cache

---

**Ready to build!** 🚀
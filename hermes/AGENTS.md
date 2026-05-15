# Hermès — AI Context for All Agents

> Universal context file for AI assistants (Claude, Cursor, GitHub Copilot, etc.)

---

## What is This Project?

**Hermès** is a React + TypeScript + Vite starter template. It's a minimal, production-ready foundation for building modern web applications with:

- ⚡ Lightning-fast HMR with Vite
- 🔒 Type safety with TypeScript
- ⚛️ Modern React 18 with hooks
- 🎨 Clean, semantic CSS
- 📦 Zero dependencies (except React)

---

## Key Technologies

| Technology | Version | Purpose |
|------------|---------|---------|
| React | 18.3+ | UI library |
| TypeScript | 5.5+ | Type safety |
| Vite | 5.3+ | Build tool |
| ESLint | 8.57+ | Code quality |

---

## File Structure

```
src/
├── main.tsx       # App entry point (ReactDOM.render)
├── App.tsx        # Root component
├── App.css        # Component styles
├── index.css      # Global styles
└── vite-env.d.ts  # Vite types
```

---

## How to Help

### When Writing Code
- Use TypeScript with strict mode
- Prefer functional components with hooks
- Keep components small and focused
- Use semantic HTML and CSS

### When Suggesting Changes
- Respect the minimal nature of this template
- Don't add unnecessary dependencies
- Keep the bundle size small
- Maintain Vite's fast HMR

### When Debugging
- Check browser console first
- Verify TypeScript compilation (`npm run build`)
- Test in dev mode (`npm run dev`)
- Check ESLint output (`npm run lint`)

---

## Common Tasks

**Add a component:**
```tsx
export function MyComponent() {
  return <div>Hello</div>;
}
```

**Add state:**
```tsx
const [count, setCount] = useState(0);
```

**Add an effect:**
```tsx
useEffect(() => {
  // Side effect here
}, [dependencies]);
```

**Style a component:**
```css
/* App.css */
.my-component {
  color: blue;
}
```

---

## Development Workflow

1. Start dev server: `npm run dev`
2. Edit files in `src/`
3. See changes instantly (HMR)
4. Build for production: `npm run build`
5. Preview build: `npm run preview`

---

## Important Notes

- This is a **minimal** template — no routing, no state management
- Uses **ESM only** — no CommonJS
- **Vite** handles all bundling — no webpack
- **TypeScript** is configured for strict mode
- **React 18** with concurrent features enabled

---

**Let's build something great!** ✨
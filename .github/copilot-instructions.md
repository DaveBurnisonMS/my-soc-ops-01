# Soc Ops: Social Bingo Game

## Development Checklist (Mandatory)

- [ ] **Lint**: `npm run lint` (ESLint passes)
- [ ] **Build**: `npm run build` (TypeScript compiles)  
- [ ] **Test**: `npm run test` (Vitest passes)

## Architecture

**Stack**: React 19 + TypeScript + Vite + Tailwind v4 + Vitest
**Pattern**: Unidirectional data flow via `useBingoGame()` hook with localStorage persistence

## Commands

```bash
npm install    # Dependencies
npm run dev    # Development server
npm run build  # Production build
```

## Code Style

**Components**: Function declarations, `interface ComponentProps`, destructured params, 20-50 lines max
**State**: All via `useBingoGame()` hook, immutable updates (`board.map()`), `useCallback` actions
**Files**: `/src/components/`, `/src/hooks/`, `/src/utils/`, `/src/types/`, `/src/data/`

## Conventions

**Naming**: Components (`*Screen`, `*Board`, `*Modal`), Hooks (`use*`), Tests (`*.test.ts`)
**TypeScript**: Strict mode, interfaces for props, domain types in `/src/types/index.ts`  
**Tailwind v4**: `@theme` config in `index.css`, custom properties (`--color-*`), bracket notation
**Testing**: Vitest + jsdom, Testing Library, behavior-focused

## Workshop Context

AI-first development patterns for VS Code Copilot Agent Mode. Architecture intentionally simple to focus on agent workflows. See [`workshop/GUIDE.md`](workshop/GUIDE.md) for lab guide.
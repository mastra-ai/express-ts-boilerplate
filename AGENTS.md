# AGENTS.md

## Build Commands

- `npm run build` - Compile TypeScript
- `npm run dev` - Development mode with watch
- `npm start` - Run production build
- No lint/test commands configured

## Code Style

- ESM project (`"type": "module"`)
- Use `type` keyword for type-only imports: `import { type Request } from "express"`
- Double quotes for strings, no semicolons
- 2-space indentation
- `SCREAMING_CASE` for constants, `camelCase` for variables
- Prefix unused parameters with underscore: `_req`
- Inline type annotations for function parameters

## TypeScript

- Strict mode enabled with `noUncheckedIndexedAccess` and `exactOptionalPropertyTypes`
- Always check for undefined when accessing arrays/objects by index
- Use explicit `type` keyword for type imports (`verbatimModuleSyntax: true`)

## Project Structure

- Source code in `src/`, compiled output in `dist/`
- Express 5.x with native ES modules

# Kurogane: React starter

A React project scaffolded with Vite for Kurogane.

## Supported languages

- `typescript`: React with TypeScript (`.tsx`), type checking via `tsc`
- `javascript`: React with JavaScript (`.jsx`), no type checking

## Usage with Kurogane CLI

```sh
kurogane new react
```

Select a language when prompted.

## Non-interactive usage

```sh
cargo generate kurogane-rs/kurogane-starter-react --name my-app --define language=typescript
```

## What's included

- React 19 entry point with `StrictMode`
- Vite with `@vitejs/plugin-react`
- `vite.config.ts` configured to build into `content/`
- Rust binary using the Kurogane runtime
- `kurogane.toml` packaging configuration

## Development

```sh
npm --prefix frontend install
npm --prefix frontend run dev  # Start Vite dev server (port 5173)
kurogane dev                   # Launch the Kurogane desktop app
```

## Bundling

```sh
npm --prefix frontend run build  # Build the frontend into frontend/dist
kurogane bundle
```

## TypeScript vs JavaScript

The TypeScript variant includes `.tsx` source files, `tsconfig.json` and type definitions. The `build` script runs `tsc -b` before Vite. The JavaScript variant uses `.jsx` files with no type checking.

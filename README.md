# Gym App — Web

The web application for Gym App, built with Next.js App Router, React, TypeScript, and Tailwind CSS.

## Requirements

- Node.js 24
- npm (until the planned pnpm migration)

## Local development

```bash
npm ci
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## Quality gates

```bash
npm run lint
npm run typecheck
npm run build
```

Pull requests to `main` and pushes to `main` run the same checks in GitHub Actions. The typecheck task runs `next typegen` first so Next.js route and layout types exist before TypeScript validation.

## Roadmap

- Adopt Nx for task orchestration and caching
- Migrate to pnpm with a committed `pnpm-lock.yaml`
- Introduce shared configuration, Oxlint, and Feature-Sliced Design
- Integrate with the separate NestJS backend via an OpenAPI-based client

The NestJS API is maintained separately at [gym-api-nestjs](https://github.com/sauron9521/gym-api-nestjs).

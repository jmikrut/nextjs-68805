# Next.js Issue #68805 Reproduction

This repo includes Payload which installs a few dependencies like Pino for you. Turbopack can't find them if installed with `pnpm` but Webpack can.

To reproduce:

1. Install dependencies with `pnpm`
1. Run `pnpm dev --turbo` to see it fail
1. Run `pnpm dev` to see it work

More info:
https://github.com/vercel/next.js/issues/68805

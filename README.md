# Nuxt Minimal Starter

Look at the [Nuxt documentation](https://nuxt.com/docs/getting-started/introduction) to learn more.

## Deploying the Site to Nostr

1) Generate the Static Site

```bash
# npm
npm run generate
```

2) Deploy the site using the config Settings.

For the first time with a fresh Nsec we still need to sign the right Blossom & Relay List Kinds.
Its easier to do this by running the normal cli wizard:
```bash
npx nsite-cli
```

```bash
npx nsite-cli upload .output/public
```

```bash
npx nsite-cli upload --relays 'wss://nos.lol,wss://relay.primal.net,wss://relay.nostr.band,wss://relay.damus.io' --servers 'https://nostrcheck.me/,https://nosto.re/' --privatekey nsec1n9cvnpstm3g69xk70jl2qj6zlljjp6eltk7czfd47ga7u3ceagcqf7k35f .output/public 
```

The website is now available on any nsite gateway, e.g.: https://npub154mx7uznec76w0wfauauqfpljl48dyzw8k23ycrah62asm0e537qxv65a5.nsite.lol

## Setup

Make sure to install dependencies:

```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install

# bun
bun install
```

## Development Server

Start the development server on `http://localhost:3000`:

```bash
# npm
npm run dev

# pnpm
pnpm dev

# yarn
yarn dev

# bun
bun run dev
```

## Production

Build the application for production:

```bash
# npm
npm run build

# pnpm
pnpm build

# yarn
yarn build

# bun
bun run build
```

Locally preview production build:

```bash
# npm
npm run preview

# pnpm
pnpm preview

# yarn
yarn preview

# bun
bun run preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.

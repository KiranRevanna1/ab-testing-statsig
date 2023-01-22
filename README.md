---
name: Experimentation with Statsig
slug: ab-testing-statsig
description: By running experiments at the edge with Statsig, you'll reduce CLS and improve performance from client-loaded experiments while analyzing impact.
framework: Next.js
useCase:
  - Edge Functions
  - Documentation
css: Tailwind
deployUrl: https://vercel.com/new/clone?repository-url=https://github.com/vercel/examples/tree/main/edge-functions/ab-testing-statsig&project-name=ab-testing-statsig&repository-name=ab-testing-statsig&env=STATSIG_SERVER_API_KEY,NEXT_PUBLIC_STATSIG_CLIENT_KEY,STATSIG_CONSOLE_API_KEY,EDGE_CONFIG,EDGE_CONFIG_ITEM_KEY&envDescription=Statsig%20API%20keys%20and%20Edge%20Config%20settings&envLink=https%3A%2F%2Fdocs.statsig.com%2Fguides%2Ffirst-feature
demoUrl: https://edge-ab-testing-statsig.vercel.app
---

# Experimentation with Statsig

This example shows how to do experimentation using Statsig, leveraging Edge Config.

## Demo

https://edge-ab-testing-statsig.vercel.app

## How to Use

You can choose from one of the following two methods to use this repository:

### One-Click Deploy

Deploy the example using [Vercel](https://vercel.com?utm_source=github&utm_medium=readme&utm_campaign=vercel-examples):

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/git/external?repository-url=https://vercel.com/new/clone?repository-url=https://github.com/vercel/examples/tree/main/edge-functions/ab-testing-statsig&project-name=ab-testing-statsig&repository-name=ab-testing-statsig&env=STATSIG_SERVER_API_KEY,NEXT_PUBLIC_STATSIG_CLIENT_KEY,STATSIG_CONSOLE_API_KEY,EDGE_CONFIG,EDGE_CONFIG_ITEM_KEY&envDescription=Statsig%20API%20keys%20and%20Edge%20Config%20settings&envLink=https%3A%2F%2Fdocs.statsig.com%2Fguides%2Ffirst-feature)

### Clone and Deploy

Execute [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app) with [npm](https://docs.npmjs.com/cli/init) or [Yarn](https://yarnpkg.com/lang/en/docs/cli/create/) to bootstrap the example:

```bash
npx create-next-app --example https://github.com/vercel/examples/tree/main/edge-functions/ab-testing-statsig
# or
yarn create next-app --example https://github.com/vercel/examples/tree/main/edge-functions/ab-testing-statsig
```

#### Set up environment variables

Log in to the [Statsig console](https://console.statsig.com/) and navigate to **Settings -> API KEYS**.
Then, copy [.env.example](./env.example) to `.env.local` and fill it in with your Client, Server and Console API keys:

```bash
cp .env.example .env.local
```

Install the [Statsig Vercel Integration](https://vercel.com/integrations/statsig) for your project.
Then fill in `.env.local` with the provided Edge Config Connection String and Edge Config Item Key.

Next, run Next.js in development mode:

```bash
npm install
npm run dev

# or

yarn
yarn dev
```

Deploy it to the cloud with [Vercel](https://vercel.com/new?utm_source=github&utm_medium=readme&utm_campaign=edge-middleware-eap) ([Documentation](https://nextjs.org/docs/deployment)).

# Code Formatting and Linting Configuration used by ForgeDev BR

## What"s included?

- [Biome](https://biomejs.dev/) for code formatting and linting;

## Setup

Install dependencies:

```bash
npm add --save-dev @biomejs/biome @forgedev-br/biome-config
```

Configure your project:

```bash
npx @biomejs/biome init
```

Extend the configuration within `biome.json` file:

```json
{
  "$schema": "https://biomejs.dev/schemas/1.9.4/schema.json",
  "extends": ["@forgedev-br/biome-config/biome"]
}
```

Add a script to package.json:

```json
"scripts": {
  "lint": "npx @biomejs/biome check src"
}
```

> **Note:** You can also run `npx @biomejs/biome check --write` to automatically fix the code.

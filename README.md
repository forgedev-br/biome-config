# Code Formatting and Linting Configuration used by ForgeDev BR

## What"s included?

- [Biome](https://biomejs.dev/) for code formatting and linting;

## Setup

Install dependencies:
```bash
npm i -D @biomejs/biome @forgedev-br/biome-config
```

Configure your project:
```bash
npx @biomejs/biome init
```

Add a script to package.json:
```json
"scripts": {
  "lint": "npx @biomejs/biome check src"
}
```

Extend the configuration within `biome.json` file:
```json
{
  "extends": ["@forgedev-br/biome-config/biome"]
}
```

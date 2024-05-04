## Intro
The plugin helps to automatically create a sitemap. A sitemap is like a map for search engines, telling them what pages you have on your site. This makes it easier for search engines to find website and urls!

## Installation
Install with [npm](https://www.npmjs.com/)
```sh
npm i -D vite-sitemap
```
or Install with [yarn](https://www.npmjs.com/package/yarn)
```sh
yarn add vite-sitemap
```
or Install with [pnpm](https://www.npmjs.com/package/pnpm)
```sh
pnpm install vite-sitemap
```

# Usage
Use the vite plugin in your project go to vite.config.js or vite.config.ts and add the following to code in vite plugin section
````js
sitemap({
        baseURL: 'www.example.com',
        urls: [
            "about",
            "privacy-policy",
            'term-and-conditions',
            ...
        ],
    }),
````
Plugin section example in vite.config.ts or js
````js
import { defineConfig } from 'vite';
import sitemap from 'vite-sitemap';

// https://vitejs.dev/config/
export default defineConfig({
  plugins: [
    sitemap({ baseURL: 'www.example.com' })
  ],
});
````
## Intro
Find the Vite plugins here. They make sitemaps for Vite projects super easy. They help users and search engines find stuff on your site easily. Makes your website better and saves you time.

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

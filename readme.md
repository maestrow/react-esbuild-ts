# [Why esbuild? Getting Started using a TypeScript / React example](https://www.youtube.com/watch?v=4rUbQJM0BgA)

npm init -y
npm i -D esbuild typescript
npm i -S react react-dom @types/react @types/react-dom
npx tsc --init --rootDir src --jsx react --target ES2015

Add `"build": "esbuild src/App.tsx --bundle --minify --sourcemap --outfile=public/bundle.js"` to package.json.
Add: 
- src/App.tsx
- public/index.html:

```html
<div id="root"></div>
<script src="bundle.js"></script>
```

npm run build


# Other ways to create typescript + react app

- https://www.metachris.com/2021/04/starting-a-typescript-project-in-2021/
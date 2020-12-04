# TS iHAT Service Template

After copying this template run

```sh
npm install --D @types/jest @typescript-eslint/eslint-plugin @typescript-eslint/parser ts-jest typescript
```

It is also recommend adding following commands in package.json 
```js
"prebuild": "npm run lint",
"build": "tsc",
"lint": "eslint . --ext .ts",
"prepublish": "rm -rf dist && npm run build",
"test": "jest --runInBand"
```
# tsconfig.json

[<= Back](../README.md)

## `tsconfig.json` for Node.js

```json
{
    "compilerOptions": {
        "module": "commonjs",
        "esModuleInterop": true,
        "allowSyntheticDefaultImports": true,
        "noEmitOnError": true,
        "outDir": "dist",
        "target": "ES6",
        "strict": true,
        "declaration": true,
        "typeRoots": ["./node_modules/@types", ".src/types/global.d.ts"]
    },
    "include": [
        "src/**/*"
    ]
}
```

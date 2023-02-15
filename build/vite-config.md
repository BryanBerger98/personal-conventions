# Vite config

## Vite config for React

```js
import path from 'path';

import react from '@vitejs/plugin-react';
import { defineConfig } from 'vite';

export default defineConfig({
    plugins: [ react() ],
    resolve: {
        alias: {
            '@components': `${ path.resolve(__dirname, 'src/components') }`,
            '@hooks': `${ path.resolve(__dirname, 'src/hooks') }`,
            '@assets': `${ path.resolve(__dirname, 'src/assets') }`,
            '@utils': `${ path.resolve(__dirname, 'src/utils') }`,
            '@contexts': `${ path.resolve(__dirname, 'src/contexts') }`,
            'public': `${ path.resolve(__dirname, 'public') }`,
        }, 
    },
});
```
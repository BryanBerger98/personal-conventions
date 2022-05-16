ESLint config:
```Javascript
// ES5 linter
module.exports = {
    'env': {
        'browser': true,
        'commonjs': true,
        'es2021': true
    },
    'extends': 'eslint:recommended',
    'parserOptions': {
        'ecmaVersion': 'latest'
    },
    'rules': {
        'indent': [
            'warn',
            4,
            {
                'SwitchCase': 1
            }
        ],
        'linebreak-style': [
            'warn',
            'unix'
        ],
        'quotes': [
            'warn',
            'single'
        ],
        'semi': [
            'warn',
            'always'
        ],
        'no-unused-vars': [
            'warn'
        ],
        'no-duplicate-imports': [
            'warn'
        ],
        'no-duplicate-case': 'warn',
        'no-constant-condition': 'warn',
        'no-func-assign': 'error',
        'no-self-assign': ['warn', {'props': true}]
    }
};
```

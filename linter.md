ESLint config:
```Javascript
// ES5 linter
module.exports = {
    'env': {
        'node': true,
        'browser': 'false',
        'commonjs': false,
        'es2021': true,
    },
    'plugins': [
        'const-case',
    ],
    'extends': 'eslint:recommended',
    'parserOptions': {
        'ecmaVersion': 'latest',
        'sourceType': 'module',
        'ecmasFeatures': {
            'jsx': false,
        },
    },
    'rules': {
        'indent': [
            'warn',
            // eslint-disable-next-line no-magic-numbers
            4,
            {
                'SwitchCase': 1,
            },
        ],
        'no-func-assign': 'error',
        'no-magic-numbers': [ 'warn', {
            'detectObjects': false,
        } ],
        // Syntax
        'semi': [ 'warn', 'always' ],
        'quotes': [ 'warn', 'single' ],
        'linebreak-style': [
            'warn',
            'unix',
        ],
        'object-curly-spacing': [ 'warn', 'always' ],
        'array-bracket-spacing': [ 'warn', 'always' ],
        'computed-property-spacing': [ 'warn', 'always' ],
        'comma-dangle': [ 'warn', {
            'arrays': 'always-multiline',
            'objects': 'always-multiline',
            'imports': 'always-multiline',
            'exports': 'always-multiline',
            'functions': 'never',
        } ],
        'arrow-spacing': 'warn',
        'key-spacing': [ 'warn', {
            'beforeColon': false,
            'afterColon': true,
            'mode': 'strict',
        } ],
        'no-multi-spaces': 'warn',
        'no-multiple-empty-lines': 'warn',
        'no-empty-function': 'warn',
        'require-await': 'error',
        'template-curly-spacing': [ 'warn', 'always' ],
        // Conditions
        'default-case': 'warn',
        'default-case-last': 'warn',
        'no-duplicate-case': 'warn',
        'no-constant-condition': 'warn',
        // Variables and constants
        'no-var': 'error',
        'no-unused-vars': 'warn',
        'no-const-assign': 'error',
        'const-case/uppercase': 'warn',
        'no-multi-assign': 'warn',
        'no-self-assign': [ 'warn', { 'props': true } ],
        // Constructors
        'new-cap': [ 'warn', {
            'capIsNew': false,
            'newIsCap': true,
        } ],
        // Text
        'valid-typeof': 'error',
        // ES6
        'no-duplicate-imports': [
            'error',
        ],
        'no-class-assign': 'error',
    },
};
```

## ESLint for React:

```javascript
module.exports = {
	env: {
		browser: true,
		node: true,
		es6: true,
	},
	extends: [
		'eslint:recommended',
		'plugin:import/errors',
		'plugin:react/recommended',
		'plugin:jsx-a11y/recommended',
	],
	plugins: [ 'jsx-a11y', 'react', 'import' ],
	parserOptions: {
		ecmaVersion: 'latest',
		sourceType: 'module',
		ecmasFeatures: {
			jsx: true,
		},
	},
	rules: {
		indent: [
			'warn',
			'tab',
			{
				SwitchCase: 1,
			},
		],
		'no-func-assign': 'error',
		'no-magic-numbers': [
			'warn',
			{
				detectObjects: false,
			},
		],
		// Syntax
		semi: [ 'warn', 'always' ],
		quotes: [ 'warn', 'single' ],
		'linebreak-style': [ 'warn', 'unix' ],
		'object-curly-spacing': [ 'warn', 'always' ],
		'array-bracket-spacing': [ 'warn', 'always' ],
		'computed-property-spacing': [ 'warn', 'always' ],
		'comma-dangle': [
			'warn',
			{
				arrays: 'always-multiline',
				objects: 'always-multiline',
				imports: 'always-multiline',
				exports: 'always-multiline',
				functions: 'never',
			},
		],
		'arrow-spacing': 'warn',
		'key-spacing': [
			'warn',
			{
				beforeColon: false,
				afterColon: true,
				mode: 'strict',
			},
		],
		'no-multi-spaces': 'warn',
		'no-multiple-empty-lines': 'warn',
		'no-empty-function': 'warn',
		'require-await': 'error',
		'template-curly-spacing': [ 'warn', 'always' ],
		// Conditions
		'default-case': 'warn',
		'default-case-last': 'warn',
		'no-duplicate-case': 'warn',
		'no-constant-condition': 'warn',
		// Variables and constants
		'no-var': 'error',
		'no-unused-vars': 'warn',
		'no-const-assign': 'error',
		'no-multi-assign': 'warn',
		'no-self-assign': [ 'warn', { props: true } ],
		// Constructors
		'new-cap': [
			'warn',
			{
				capIsNew: false,
				newIsCap: true,
			},
		],
		// Text
		'valid-typeof': 'error',
		// ES6
		'no-duplicate-imports': [ 'error' ],
		'no-class-assign': 'error',
		// React
		'react/prop-types': 1,
		'react/react-in-jsx-scope': 'off',
	},
	settings: {
		'react': {
			version: 'detect',
		},
		'import/resolver': {
			'alias': {
				'extensions': [ '.js', '.jsx' ],
				'map': [
					[ 'src', './src' ],
					[ 'app', './src' ],
				],
			},
		},
	},
};


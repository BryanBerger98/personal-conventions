# ESLint rules for React projects

[<= Back](../../README.md)

The following `javascript` code should be set into the `.eslintrc.cjs` file:

```js
module.exports = {
	'env': {
		'browser': true,
		'node': true,
		'es2022': true,
	},
	'extends': [
		'eslint:recommended',
		'plugin:react/recommended',
		'plugin:import/errors',
		'plugin:jsx-a11y/recommended',
	],
	'parserOptions': {
		'ecmaFeatures': { 'jsx': true },
		'ecmaVersion': 'latest',
		'sourceType': 'module',
		'project': './jsconfig.json',
	},
	'plugins': [
		'react',
		'jsx-a11y',
		'import',
	],
	'rules': {
		'indent': [
			'warn',
			'tab',
			{ 'SwitchCase': 1 },
		],
		'no-func-assign': 'error',
		'no-magic-numbers': [
			'warn',
			{
				'detectObjects': false,
				'ignoreArrayIndexes': true,
				'ignoreDefaultValues': true,
				'ignoreClassFieldInitialValues': true,
			},
		],
		// Syntax
		'semi': [ 'warn', 'always' ],
		'quotes': [ 'warn', 'single' ],
		'linebreak-style': [ 'warn', 'unix' ],
		'array-bracket-spacing': [ 'warn', 'always' ],
		'computed-property-spacing': [ 'warn', 'always' ],
		'comma-dangle': [
			'warn',
			{
				'arrays': 'always-multiline',
				'objects': 'always-multiline',
				'imports': 'always-multiline',
				'exports': 'always-multiline',
				'functions': 'never',
			},
		],
		'arrow-spacing': 'warn',
		'key-spacing': [
			'warn',
			{
				'beforeColon': false,
				'afterColon': true,
				'mode': 'strict',
			},
		],
		'no-multi-spaces': 'warn',
		'no-multiple-empty-lines': 'warn',
		'no-empty-function': 'warn',
		'require-await': 'error',
		'template-curly-spacing': [ 'warn', 'always' ],
		'brace-style': [ 'warn', '1tbs' ],
		'no-param-reassign': [
			'error',
			{ 'props': false },
		],
		'prefer-destructuring': [
			'warn',
			{
				'VariableDeclarator': {
					'array': true,
					'object': true,
				},
				'AssignmentExpression': {
					'array': true,
					'object': false,
				},
			},
			{ 'enforceForRenamedProperties': false },
		],
		'one-var-declaration-per-line': [ 'error', 'always' ],
		'one-var': [ 'error', 'never' ],
		'rest-spread-spacing': [ 'warn', 'never' ],
		// Objects
		'object-curly-spacing': [ 'warn', 'always' ],
		'object-property-newline': 'warn',
		'object-curly-newline': [
			'warn',
			{
				'ObjectExpression': {
					'multiline': true,
					'minProperties': 2,
				},
				'ObjectPattern': { 'multiline': true },
				'ImportDeclaration': 'never',
				'ExportDeclaration': {
					'multiline': true,
					'minProperties': 3,
				},
			},
		],
		'prefer-object-has-own': 'warn',
		'prefer-object-spread': 'warn',
		// Functions
		'func-names': 'off',
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
		'no-self-assign': [ 'warn', { 'props': true } ],
		// Constructors
		'new-cap': [
			'warn',
			{
				'capIsNew': false,
				'newIsCap': true,
			},
		],
		// Text
		'valid-typeof': 'error',
		// ES6
		'no-duplicate-imports': [ 'error' ],
		'no-class-assign': 'error',
		'object-shorthand': 'off',
		// React
		'react/prop-types': 1,
		'react/react-in-jsx-scope': 'off',
		'react/jsx-filename-extension': [ 1, { 'extensions': [ '.js', '.jsx' ] } ],
		'react/forbid-prop-types': 2,
		'react/no-access-state-in-setstate': 'error',
		'react/jsx-one-expression-per-line': 'off',
		'react/destructuring-assignment': 'warn',
		'react/no-unescaped-entities': 'off',
		'react/jsx-props-no-spreading': 'off',
		'react/state-in-constructor': [ 1, 'always' ],
		'react/jsx-uses-react': 'off',
		'react/jsx-uses-vars': 'warn',
		'react/function-component-definition': [
			1,
			{
				'namedComponents': 'arrow-function',
				'unamedComponents': 'arrow-function',
			},
		],
		// JSX
		'jsx-a11y/no-static-element-interactions': 'error',
		'jsx-a11y/anchor-is-valid': 'off',
		'jsx-a11y/mouse-events-have-key-events': 'off',
		'jsx-a11y/click-events-have-key-events': 'off',
		'jsx-a11y/no-noninteractive-element-interactions': 'off',
		// Imports
		'import/order': [
			'warn',
			{
				'groups': [ 'builtin', 'external', 'internal', 'parent', 'sibling', 'index', 'unknown' ],
				'pathGroups': [
					{
						'pattern': '{.,..}/*.css',
						'group': 'sibling',
						'position': 'after',
					},
				],
				'alphabetize': {
					'order': 'asc',
					'caseInsensitive': true,
				},
				'newlines-between': 'always',
			},
		],
	},
	'settings': {
		'react': { 'version': 'detect' },
		'import/resolver': {
			'alias': {
				'extensions': [ '.js', '.jsx' ],
				'map': [
					[ '@assets', './src/assets' ],
					[ '@hooks', './src/hooks' ],
					[ '@components', './src/components' ],
					[ '@contexts', './src/contexts' ],
					[ '@utils', './src/utils' ],
					[ 'public', './public' ],
				],
			},
		}, 
	},
};
```

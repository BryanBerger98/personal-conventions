# jsconfig.json

[<= Back](../README.md)

## `jsconfig.json` for React

```json
{
	"compilerOptions": {
		"baseUrl": ".",
		"target": "ES6",
		"moduleResolution": "node",
		"paths": {
			"@assets/*": ["./src/assets/*"],
			"@hooks/*": ["./src/hooks/*"],
			"@components/*": ["./src/components/*"],
			"@contexts/*": ["./src/contexts/*"],
			"@utils/*": ["./src/utils/*"],
			"public/*": ["./public/*"]
		}
	},
	"include": ["src"],
	"exclude": ["dist", "node_modules"]
}
```

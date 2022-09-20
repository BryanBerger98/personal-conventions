# VSCode Settings

## `settings.json`:

```JSON
{
	// EXTENSIONS
	"extensions.ignoreRecommendations": true,

	// WORKBENCH
	"workbench.productIconTheme": "fluent-icons",
	"workbench.colorTheme": "One Dark Pro Mix",
	"workbench.iconTheme": "vscode-icons",
	"workbench.startupEditor": "none",

	// TERMINAL
	"terminal.integrated.tabs.enabled": true,
	"terminal.integrated.env.osx": {
		"FIG_NEW_SESSION": "1"
	},

	// LIVRESHARE
	"liveshare.autoShareServers": false,
	"liveshare.openSharedServers": false,

	// PRETTIER
	"prettier.semi": true,
	"prettier.tabWidth": 4,
	"prettier.singleQuote": true,
	"prettier.trailingComma": "all",
	"prettier.bracketSpacing": true,
	"prettier.endOfLine": "lf",
	"prettier.useTabs": true,
	"prettier.printWidth": 200,
	"prettier.jsxSingleQuote": true,
	"prettier.bracketSameLine": false,
	"prettier.arrowParens": "always",

	// EDITOR
	"editor.tabSize": 4,
	"editor.insertSpaces": false,
	"editor.detectIndentation": false,
	"editor.linkedEditing": true,
	"editor.accessibilitySupport": "off",
	"editor.defaultFormatter": "esbenp.prettier-vscode",
	"editor.formatOnSave": true,
	"[javascript]": {
		"editor.formatOnSave": false,
		"editor.codeActionsOnSave": {
			"source.fixAll": true
		}
	},
	"[javascriptreact]": {
		"editor.formatOnSave": false,
		"editor.codeActionsOnSave": {
			"source.fixAll": true
		}
	},
	"[typescript]": {
		"editor.formatOnSave": false,
		"editor.codeActionsOnSave": {
			"source.fixAll": true
		}
	},

	// ESLINT
	"eslint.workingDirectories": [{ "mode": "auto" }],

	// OTHERS
	"emmet.includeLanguages": {
		"javascript": "javascriptreact"
	},
	"security.workspace.trust.untrustedFiles": "open",
	"files.associations": {
		"*.ejs": "html",
		"*.tmpl": "html",
		"*.css": "css",
		"*.scss": "scss",
		"*.js": "javascript",
		"*.jsx": "javascriptreact",
		"*.ts": "typescript",
		"*.tsx": "typescriptreact"
	},
	"go.addTags": {
		"tags": "json",
		"options": "json=omitempty",
		"promptForTags": false,
		"transform": "snakecase",
		"template": ""
	},
	"window.zoomLevel": 3,
	"vsicons.dontShowNewVersionMessage": true,
	"explorer.compactFolders": false,
	"editor.minimap.autohide": true,
	"editor.minimap.enabled": false,
	"javascript.updateImportsOnFileMove.enabled": "always"
}
```

# VSCode Settings

[<= Back](../README.md)

## `settings.json`

```JSON
{
	"extensions.ignoreRecommendations": true,

	// WINDOW
	"window.zoomLevel": 2,
	// "window.autoDetectColorScheme": true,
	// "window.autoDetectHighContrast": true,

	// WORKBENCH
	"workbench.productIconTheme": "fluent-icons",
	"workbench.iconTheme": "vscode-icons",
	"workbench.startupEditor": "none",
	"workbench.tree.indent": 12,
	"workbench.tree.renderIndentGuides": "always",
	"workbench.editor.enablePreview": false,
	"workbench.editor.highlightModifiedTabs": true,

	// TERMINAL
	"terminal.integrated.tabs.enabled": true,
	"terminal.integrated.env.osx": {
		"FIG_NEW_SESSION": "1"
	},

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
	"prettier.singleAttributePerLine": false,

	// EDITOR
	"editor.fontFamily": "'JetBrains Mono', Consolas, Menlo, Monaco, 'Courier New', monospace",
	"editor.fontLigatures": false,
	"editor.minimap.autohide": true,
	"editor.minimap.enabled": false,
	"editor.tabSize": 4,
	"editor.insertSpaces": false,
	"editor.detectIndentation": false,
	"editor.linkedEditing": true,
	"editor.accessibilitySupport": "off",
	"editor.defaultFormatter": "esbenp.prettier-vscode",
	"editor.formatOnSave": true,
	"editor.formatOnPaste": false,
	"editor.occurrencesHighlight": true,
	"editor.acceptSuggestionOnCommitCharacter": false,
	"editor.suggest.insertMode": "replace",
	"editor.renderWhitespace": "trailing",
	"editor.inlayHints.enabled": "offUnlessPressed",
	"[javascript]": {
		"editor.formatOnSave": false,
		"editor.codeActionsOnSave": {
			"source.fixAll": true
		},
		"javascript.preferences.quoteStyle": "single"
	},
	"[javascriptreact]": {
		"editor.formatOnSave": false,
		"editor.codeActionsOnSave": {
			"source.fixAll": true
		},
		"javascript.autoClosingTags": true,
		"javascript.preferences.quoteStyle": "single",
		"javascript.preferences.jsxAttributeCompletionStyle": "none",
		"javascript.preferences.importModuleSpecifier": "shortest",
		"javascript.preferences.importModuleSpecifierEnding": "minimal"
	},
	"[typescript]": {
		"editor.formatOnSave": false,
		"editor.codeActionsOnSave": {
			"source.fixAll": true
		},
		"typescript.preferences.quoteStyle": "single"
	},
	"[typescriptreact]": {
		"editor.formatOnSave": false,
		"editor.codeActionsOnSave": {
			"source.fixAll": true
		},
		"typescript.autoClosingTags": true,
		"typescript.preferences.quoteStyle": "single",
		"typescript.preferences.jsxAttributeCompletionStyle": "none",
		"typescript.preferences.importModuleSpecifier": "shortest",
		"typescript.preferences.importModuleSpecifierEnding": "minimal"
	},
	"[html]": {
		"editor.formatOnSave": true
	},
	"[json]": {
		"editor.formatOnSave": true,
		"editor.quickSuggestions": {
			"strings": true
		},
		"editor.suggest.insertMode": "replace"
	},
	"[jsonc]": {
		"editor.formatOnSave": true,
		"editor.quickSuggestions": {
			"strings": true
		},
		"editor.suggest.insertMode": "replace"
	},
	"[markdown]": {
		"editor.unicodeHighlight.ambiguousCharacters": false,
		"editor.unicodeHighlight.invisibleCharacters": false,
		"editor.wordWrap": "on",
		"editor.quickSuggestions": {
			"comments": "on",
			"strings": "on",
			"other": "on"
		},
		"editor.formatOnSave": false,
		"editor.codeActionsOnSave": {
			"source.fixAll": true
		}
	},

	// HTML
	"html.format.templating": false,
	"html.validate.scripts": false,
	"htmlhint.options": {
		"spec-char-escape": false,
		"doctype-first": false
	},

	// JavaScript
	"javascript.updateImportsOnFileMove.enabled": "always",
	"javascript.autoClosingTags": true,
	"javascript.format.enable": true,
	"javascript.format.semicolons": "insert",
	"javascript.preferences.quoteStyle": "single",

	// EMMET
	"emmet.includeLanguages": {
		"javascript": "javascriptreact",
		"ejs": "html"
	},
	"emmet.triggerExpansionOnTab": false,

	// TAILWIND
	"tailwindCSS.emmetCompletions": true,

	// ESLINT
	"eslint.workingDirectories": [{ "mode": "auto" }],

	// FILES
	"files.associations": {
		"*.ejs": "html",
		"*.tmpl": "html",
		"*.css": "tailwindcss",
		"*.scss": "scss",
		"*.js": "javascript",
		"*.jsx": "javascriptreact",
		"*.ts": "typescript",
		"*.tsx": "typescriptreact"
	},
	"files.exclude": {
		"**/.git": true,
		"**/.svn": true,
		"**/.hg": true,
		"**/CVS": true,
		"**/.DS_Store": true,
		"**/Thumbs.db": true
	},
	"files.defaultLanguage": "markdown",

	// EXPLORER
	"explorer.autoReveal": true,
	"explorer.confirmDragAndDrop": false,
	"explorer.confirmDelete": true,
	"explorer.confirmUndo": "default",
	"explorer.compactFolders": false,

	// OTHERS
	"security.workspace.trust.untrustedFiles": "open",
	// "go.addTags": {
	// 	"tags": "json",
	// 	"options": "json=omitempty",
	// 	"promptForTags": false,
	// 	"transform": "snakecase",
	// 	"template": ""
	// },
	"vsicons.dontShowNewVersionMessage": true,
	"vsicons.presets.hideExplorerArrows": false,
	// "liveshare.openSharedServers": false,
	// "liveshare.autoShareServers": false,
	// "liveServer.settings.donotShowInfoMsg": true,
	"codesnap.backgroundColor": "rgba(0, 0, 0, 0)",
	"codesnap.boxShadow": "rgba(0, 0, 0, 0.55) 0px 10px 32px",
	"codesnap.showWindowTitle": false,
	"codesnap.roundedCorners": true,
	"codesnap.showWindowControls": false,
	"task.allowAutomaticTasks": "off",
	"better-comments.tags": [
		{
			"tag": "!",
			"color": "#FF2D00",
			"strikethrough": false,
			"underline": false,
			"backgroundColor": "transparent",
			"bold": false,
			"italic": false
		},
		{
			"tag": "?",
			"color": "#3498DB",
			"strikethrough": false,
			"underline": false,
			"backgroundColor": "transparent",
			"bold": false,
			"italic": false
		},
		{
			"tag": "//",
			"color": "#474747",
			"strikethrough": true,
			"underline": false,
			"backgroundColor": "transparent",
			"bold": false,
			"italic": false
		},
		{
			"tag": "todo",
			"color": "#FF8C00",
			"strikethrough": false,
			"underline": false,
			"backgroundColor": "transparent",
			"bold": false,
			"italic": false
		},
		{
			"tag": "fixme",
			"color": "#ffde1f",
			"strikethrough": false,
			"underline": false,
			"backgroundColor": "transparent",
			"bold": false,
			"italic": false
		},
		{
			"tag": "*",
			"color": "#98C379",
			"strikethrough": false,
			"underline": false,
			"backgroundColor": "transparent",
			"bold": false,
			"italic": false
		}
	],
	"github.copilot.enable": {
		"*": true,
		"plaintext": false,
		"markdown": false,
		"scminput": false
	},
	"git.confirmSync": false,
	"window.titleBarStyle": "custom",
	"workbench.colorTheme": "One Dark Pro"
}
```

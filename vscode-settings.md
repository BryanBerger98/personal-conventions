# VSCode Settings

## `settings.json`:

```JSON
{
  // EXTENSIONS
  "extensions.ignoreRecommendations": true,

  // WORKBENCH
  "workbench.productIconTheme": "fluent-icons",
  "workbench.colorTheme" : "One Dark Pro Mix",
  "workbench.iconTheme": "vscode-icons",
  "workbench.startupEditor" : "none",

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
  "prettier.jsxBracketSameLine": false,
  "prettier.arrowParens": "always",

  // EDITOR
  "editor.tabSize": 4,
  "editor.insertSpaces": false,
  "editor.detectIndentation": false,
  "editor.linkedEditing": true,
  "editor.accessibilitySupport" : "off",
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "[javascript]": {
    "editor.formatOnSave": true
  },
  "[typescript]": {
    "editor.formatOnSave": true
  },

  // ESLINT
  "eslint.workingDirectories": [
    {"mode": "auto"}
  ],

  // OTHERS
  "emmet.includeLanguages" : {
    "javascript" : "javascriptreact"
  },
  "security.workspace.trust.untrustedFiles" : "open",  
  "files.associations": {
    "*.ejs": "html",
    "*.tmpl": "html"
  },
  "go.addTags": {
    "tags": "json",
    "options": "json=omitempty",
    "promptForTags": false,
    "transform": "snakecase",
    "template": ""
  },
  "window.zoomLevel": 1,
  "vsicons.dontShowNewVersionMessage": true,
  "explorer.compactFolders": false,
}
```

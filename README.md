# VS Code Settings

# Font

* [Anonymous Pro](https://www.marksimonson.com/fonts/view/anonymous-pro)

## Themes/Color

* [City Lights](https://marketplace.visualstudio.com/items?itemName=Yummygum.city-lights-theme)

## Extensions

### Theme / Editor Experience

- **[Beautify](https://marketplace.visualstudio.com/items?itemName=HookyQR.beautify)**  
  Beautify code in place for VS Code.
  
- **[City Lights Icon Package](https://marketplace.visualstudio.com/items?itemName=Yummygum.city-lights-icon-vsc)**  
  A gorgeous set of icons for visual clarity in the editor.
  
- **[City Lights Theme](https://marketplace.visualstudio.com/items?itemName=Yummygum.city-lights-theme)**  
  A modern, dark theme for a visually comfortable coding experience.

- **[FontSize Shortcuts](https://marketplace.visualstudio.com/items?itemName=fosshaas.fontsize-shortcuts)**  
  Allows changing the editor font size with keyboard shortcuts.

- **[indent-rainbow](https://marketplace.visualstudio.com/items?itemName=oderwat.indent-rainbow)**  
  Adds rainbow colors to indentation levels for better readability.

- **[Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)**  
  An opinionated code formatter supporting many languages.

### Useful Tools

- **[Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)**  
  Checks and highlights spelling errors in source code.

- **[GitLens — Git supercharged](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)**  
  Enhances Git integration in VS Code with history visualization and more.

- **[Go to Spec](https://marketplace.visualstudio.com/items?itemName=Lourenci.go-to-spec)**  
  Easily switch between code and its spec file.

- **[Import Cost](https://marketplace.visualstudio.com/items?itemName=wix.vscode-import-cost)**  
  Displays the size of imports and requires directly in the editor.

- **[Multiple Cursor Case Preserve](https://marketplace.visualstudio.com/items?itemName=Cardinal90.multi-cursor-case-preserve)**  
  Preserves case when editing with multiple cursors.

- **[Path Autocomplete](https://marketplace.visualstudio.com/items?itemName=ionutvmi.path-autocomplete)**  
  Offers path auto-completion for files and directories in code.

- **[Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)**  
  Autocompletes file paths in the editor.

- **[Version Lens](https://marketplace.visualstudio.com/items?itemName=pflannery.vscode-versionlens)**  
  Shows the latest version of dependencies for package managers like npm.

### Languages and Libraries

- **[Babel JavaScript](https://marketplace.visualstudio.com/items?itemName=mgmcdermott.vscode-language-babel)**  
  VSCode syntax highlighting for modern JavaScript.

- **[colorize](https://marketplace.visualstudio.com/items?itemName=kamikillerto.vscode-colorize)**  
  Visualizes CSS colors directly in the code.

- **[ES7+ React/Redux/React-Native snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)**  
  Provides snippets for React, Redux, and React-Native development.

- **[GraphQL: Language Feature Support](https://marketplace.visualstudio.com/items?itemName=GraphQL.vscode-graphql)**  
  Adds autocompletion, error checking, and jump-to-definition for GraphQL.

- **[GraphQL: Syntax Highlighting](https://marketplace.visualstudio.com/items?itemName=GraphQL.vscode-graphql-syntax)**  
  Provides syntax highlighting for `.graphql` files and embedded GraphQL.

- **[Liquid](https://marketplace.visualstudio.com/items?itemName=sissel.shopify-liquid)**  
  Essential extension for Liquid syntax, widely used for Shopify development.

- **[Liquid Languages Support](https://marketplace.visualstudio.com/items?itemName=neilding.language-liquid)**  
  Provides syntax highlighting and language features for Liquid templates.

- **[Ruby](https://marketplace.visualstudio.com/items?itemName=rebornix.Ruby)**  
  Adds language support and debugging capabilities for Ruby in VS Code.

- **[Ruby Solargraph](https://marketplace.visualstudio.com/items?itemName=castwide.solargraph)**  
  Provides code completion, documentation, and static analysis for Ruby.

- **[Sass (.sass only)](https://marketplace.visualstudio.com/items?itemName=Syler.sass-indented)**  
  Adds syntax highlighting and linting for Sass files using indented syntax.

- **[Stylelint](https://marketplace.visualstudio.com/items?itemName=stylelint.vscode-stylelint)**  
  Lints stylesheets and ensures they conform to a consistent code style.

- **[VSCode Ruby](https://marketplace.visualstudio.com/items?itemName=wingrunr21.vscode-ruby)**  
  Adds Ruby syntax highlighting, snippets, and language configuration.

# Settings

```json
{
  // Language-specific editor settings
  "[html]": {
    "editor.defaultFormatter": "vscode.html-language-features"
  },
  "[liquid]": {
    "editor.defaultFormatter": "vscode.html-language-features"
  },
  "[markdown]": {
    "editor.quickSuggestions": {
      "comments": "off",
      "other": "off",
      "strings": "off"
    },
    "editor.wordWrap": "on"
  },

  // Editor appearance and behavior
  "editor.fontFamily": "Anonymous Pro",
  "editor.fontLigatures": true,
  "editor.fontSize": 14,
  "editor.lineHeight": 0,
  "editor.tabSize": 2,
  "editor.scrollBeyondLastLine": false,
  "editor.renderWhitespace": "boundary",
  "editor.accessibilitySupport": "off",
  "editor.bracketPairColorization.enabled": false,
  "editor.stickyScroll.enabled": true,
  "editor.linkedEditing": true,

  // Code formatting and editing
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSaveMode": "modificationsIfAvailable",
  "editor.formatOnType": true,
  "editor.codeActionsOnSave": {
    "source.organizeImports": "explicit"
  },
  "editor.tabCompletion": "on",

  // Language validation and linting
  "css.lint.float": "error",
  "css.validate": false,
  "scss.validate": false,
  "stylelint.validate": [
    "sass",
    "scss"
  ],
  "files.associations": {
    "*.html": "liquid"
  },

  // Git integration and settings
  "git.autofetch": true,
  "git.confirmSync": false,
  "git.enableSmartCommit": true,

  // GitLens settings
  "gitlens.plusFeatures.enabled": false,
  "gitlens.codeLens.recentChange.enabled": false,
  "gitlens.codeLens.authors.enabled": false,

  // Explorer and file settings
  "explorer.confirmDelete": false,
  "explorer.confirmDragAndDrop": false,

  // Emmet settings for different languages
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "liquid": "html",
    "twig": "html",
    "erb": "html",
    "ruby": "html"
  },

  // Diff editor settings
  "diffEditor.ignoreTrimWhitespace": false,

  // JavaScript/TypeScript settings
  "javascript.updateImportsOnFileMove.enabled": "always",

  // Ruby-specific settings
  "ruby.intellisense": "rubyLocate",

  // Workbench appearance and behavior
  "workbench.colorTheme": "City Lights",
  "workbench.iconTheme": "city-lights-icons-vsc",
  "workbench.startupEditor": "none",
  "workbench.editor.empty.hint": "hidden",

  // Terminal environment settings
  "terminal.integrated.env.osx": {
    "FIG_NEW_SESSION": "1"
  },

  // Security settings
  "security.workspace.trust.untrustedFiles": "open"
}
```

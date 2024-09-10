# VS Code Settings

# Font

* [Anonymous Pro](https://www.marksimonson.com/fonts/view/anonymous-pro)

## Themes/Color

* [City Lights](https://marketplace.visualstudio.com/items?itemName=Yummygum.city-lights-theme)

## Extensions

* Theme / Editor Experience
  * [FontSize ShortCuts](https://marketplace.visualstudio.com/items?itemName=fosshaas.fontsize-shortcuts)
    * Change the font size with keyboard shortcuts.
  * [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons)
    * Nice / colorful icons for many different file types
  * [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
    * Integrates ESLint JS
  * [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
    * Automatically format javascript, JSON, CSS, Sass
  * [Paste JSON as Code](https://marketplace.visualstudio.com/items?itemName=quicktype.quicktype)
    * Auto generate TypeScript (and other languages) types from JSON data., and HTML files.
  * [PostCSS Intellisense and Highlighting](https://marketplace.visualstudio.com/items?itemName=vunguyentuan.vscode-postcss)
    * Works better than the other more popular one of a similar name.
  * [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
    * Spell check markdown, comments and variable names.
  * [Pretty TypeScript Errors](https://marketplace.visualstudio.com/items?itemName=yoavbls.pretty-ts-errors)
    * Makes TS errors more human readable.
* Useful Tools
  * [Paste JSON as Code](https://marketplace.visualstudio.com/items?itemName=quicktype.quicktype)
    * Auto generate TypeScript (and other languages) types from JSON data.
  * [Code Snap](https://marketplace.visualstudio.com/items?itemName=adpyke.codesnap)
    * Take pictures of code with your VS Code Theme / Font settings.
  * [Thunder Client](https://marketplace.visualstudio.com/items?itemName=rangav.vscode-thunder-client)
    * Make HTTP requests from inside VS Code (similar to Postman / Insomnia).
* Languages and Libraries
  * [XML Tools](https://marketplace.visualstudio.com/items?itemName=DotJoshJohnson.xml)
    * XML Formatting, XQuery, and XPath Tools for Visual Studio Code.
  * [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)
    * Intelligent Tailwind CSS tooling for VS Code.
  * React
    * [ES7+ React/Redux/React-Native snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)
      * Extensions for React, React-Native and Redux in JS/TS with ES7+ syntax. Customizable. Built-in integration with prettier.
    * [CSS to JSS](https://marketplace.visualstudio.com/items?itemName=infarkt.css-to-jss)
      * Convert CSS to JSS
    * [CSS in JS](https://marketplace.visualstudio.com/items?itemName=paulmolluzzo.convert-css-in-js)
      * Get syntax highlighting when working with CSS in JS template strings.
    * [vscode-styled-components](https://marketplace.visualstudio.com/items?itemName=styled-components.vscode-styled-components)
      * Syntax highlighting for styled-components.
  * [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar)
    * Language support for Vue 3
  * [Svelte for VS Code](https://marketplace.visualstudio.com/items?itemName=svelte.svelte-vscode)
    * Svelte language support for VS Code.
  * [Prisma](https://marketplace.visualstudio.com/items?itemName=Prisma.prisma)
    * Adds syntax highlighting, formatting, auto-completion, jump-to-definition and linting for .prisma files.
  * [htmx-tags](https://marketplace.visualstudio.com/items?itemName=otovo-oss.htmx-tags)
    * Provides HTMX tag completion in HTML files in VSCode
  * [Markdown Mermaid Preview](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid)
    * View Mermaid diagrams when previewing Markdown.

### Extension package names for easy install

```
nur.just-black
fosshaas.fontsize-shortcuts
vscode-icons-team.vscode-icons
dbaeumer.vscode-eslint
esbenp.prettier-vscode
quicktype.quicktype
vunguyentuan.vscode-postcss
streetsidesoftware.code-spell-checker
yoavbls.pretty-ts-errors
quicktype.quicktype
adpyke.codesnap
rangav.vscode-thunder-client
DotJoshJohnson.xml
bradlc.vscode-tailwindcss
dsznajder.es7-react-js-snippets
infarkt.css-to-jss
paulmolluzzo.convert-css-in-js
styled-components.vscode-styled-components
Vue.volar
svelte.svelte-vscode
Prisma.prisma
otovo-oss.htmx-tags
bierner.markdown-mermaid
```

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

## Past Themes

* Original theme I use in some videos:
  * [Seti-Monokai](https://marketplace.visualstudio.com/items?itemName=SmukkeKim.theme-setimonokai)
* I used this darker modification of the above theme for a few videos:
  * [Seti-Black](https://marketplace.visualstudio.com/items?itemName=bobsparadox.seti-black)

# VSCode
Users Settings:
```js
{
    "explorer.confirmDelete": false,
    "git.enableSmartCommit": true,
    "git.confirmSync": false,
    "explorer.confirmDragAndDrop": false,
    "gitlens.advanced.messages": {
        "suppressShowKeyBindingsNotice": true,
        "suppressWelcomeNotice": true
    },
    "workbench.iconTheme": "material-icon-theme",
    "editor.fontFamily": "Operator Mono, Fira Code, Menlo, Monaco, 'Courier New', monospace",
    "editor.fontLigatures": true,
    "editor.minimap.enabled": false,
    "editor.formatOnSave": true,
    // The Cursive font is operator Mono, it's $200 and you need to buy it to get the cursive
    "editor.fontSize": 16,
    "editor.lineHeight": 25,
    "editor.letterSpacing": 0.5,
    "files.trimTrailingWhitespace": true,
    "editor.fontWeight": "400",
    "editor.cursorStyle": "block",
    "editor.cursorBlinking": "solid",
    // Very important: Install this plugin: https://github.com/be5invis/vscode-custom-css
    // You'll need to change this to a file URI scheme on your computer: https://en.wikipedia.org/wiki/File_URI_scheme
    // Mac/Linux: file:///Users/YOUR-PC-USERNAME/.vscodestyles.css
    // Windows: file:///C:/Users/YOUR-PC-USERNAME/.vscodestyles.css
    "vscode_custom_css.imports": [
        "file:///Users/efichot/Documents/styles.css"
    ],
    // "[javascript]": {
    //     "editor.formatOnSave": false
    // },
    "eslint.autoFixOnSave": true,
    "eslint.alwaysShowStatus": true,
    // "prettier.disableLanguages": [
    //     "js"
    // ],
    "files.autoSave": "onFocusChange",
    "editor.tabSize": 2,
    "workbench.colorTheme": "Oceanic Next (dimmed bg)",
    "editor.acceptSuggestionOnEnter": false,
    "editor.acceptSuggestionOnCommitCharacter": false,
    "workbench.startupEditor": "newUntitledFile",
    "git.autofetch": true,
    "javascript.updateImportsOnFileMove.enabled": "always",
    "prettier.semi": false,
    "prettier.singleQuote": true,
    "prettier.eslintIntegration": true,
}
```
Keybindings.json
```js
// Place your key bindings in this file to overwrite the defaults
[{
        "key": "a",
        "command": "explorer.newFile",
        "when": "filesExplorerFocus && !inputFocus"
    }, {

    },
    {
        "key": "shift+a",
        "command": "explorer.newFolder",
        "when": "filesExplorerFocus && !inputFocus"
    },
    {
        "key": "backspace",
        "command": "deleteFile",
        "when": "filesExplorerFocus && !inputFocus"
    },
    {
        "key": "alt+cmd+backspace",
        "command": "-deleteFile",
        "when": "explorerViewletVisible && filesExplorerFocus"
    }
]
```
.eslintrc
```js
{
  "extends": ["airbnb", "prettier", "prettier/react"],
  "parser": "babel-eslint",
  "parserOptions": {
    "ecmaVersion": 8,
    "ecmaFeatures": {
      "experimentalObjectRestSpread": true,
      "impliedStrict": true,
      "classes": true
    }
  },
  "env": {
    "browser": true,
    "node": true,
    "jquery": true
  },
  "rules": {
    "no-unused-vars": [
      1,
      {
        "argsIgnorePattern": "res|next|^err|props"
      }
    ],
    "arrow-body-style": [2, "as-needed"],
    "no-param-reassign": [
      2,
      {
        "props": false
      }
    ],
    "no-console": 0,
    "import": 0,
    "func-names": 0,
    "space-before-function-paren": 0,
    "comma-dangle": 0,
    "max-len": 0,
    "import/extensions": 0,
    "no-underscore-dangle": 0,
    "consistent-return": 0,
    "react/display-name": 0,
    "react/react-in-jsx-scope": 0,
    "react/prefer-stateless-function": 0,
    "react/forbid-prop-types": 0,
    "react/no-unescaped-entities": 0,
    "react/jsx-filename-extension": [
      1,
      {
        "extensions": [".js", ".jsx"]
      }
    ],
    "radix": 0,
    "no-shadow": [
      2,
      {
        "hoist": "all",
        "allow": ["resolve", "reject", "done", "next", "err", "error"]
      }
    ],
    "quotes": [
      2,
      "single",
      {
        "avoidEscape": true,
        "allowTemplateLiterals": true
      }
    ],
    "prettier/prettier": [
      "error",
      {
        "trailingComma": "es5",
        "singleQuote": true,
        "printWidth": 120,
        "semi": false
      }
    ],
    "jsx-a11y/href-no-hash": "off",
    "jsx-a11y/anchor-is-valid": [
      "warn",
      {
        "aspects": ["invalidHref"]
      }
    ]
  },
  "plugins": ["eslint-plugin-html", "prettier"]
}

```

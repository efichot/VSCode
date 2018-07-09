# VSCode
Users Settings
```js
{
    "explorer.confirmDelete": false,
    "git.enableSmartCommit": true,
    "git.confirmSync": false,
    "explorer.confirmDragAndDrop": false,
    "gitlens.advanced.messages": {
        "suppressCommitHasNoPreviousCommitWarning": false,
        "suppressCommitNotFoundWarning": false,
        "suppressFileNotUnderSourceControlWarning": false,
        "suppressGitVersionWarning": false,
        "suppressLineUncommittedWarning": false,
        "suppressNoRepositoryWarning": false,
        "suppressUpdateNotice": false,
        "suppressWelcomeNotice": true
    },
    "workbench.iconTheme": "material-icon-theme",
    "editor.renderWhitespace": "all",
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
    "editor.cursorStyle": "line",
    "editor.cursorBlinking": "solid",
    // Very important: Install this plugin: https://github.com/be5invis/vscode-custom-css
    // You'll need to change this to a file URI scheme on your computer: https://en.wikipedia.org/wiki/File_URI_scheme
    // Mac/Linux: file:///Users/YOUR-PC-USERNAME/.vscodestyles.css
    // Windows: file:///C:/Users/YOUR-PC-USERNAME/.vscodestyles.css
    "vscode_custom_css.imports": [
        "file:///Users/efichot/Documents/styles.css"
    ],
    "[javascript]": {
        "editor.formatOnSave": false
    },
    "eslint.autoFixOnSave": true,
    "eslint.alwaysShowStatus": true,
    "prettier.disableLanguages": [
        "js"
    ],
    "files.autoSave": "onFocusChange",
    "editor.tabSize": 2,
    "workbench.colorTheme": "Operator Mono Dark Theme",
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
        "when": "explorerViewletVisible && filesExplorerFocus"
    },
    {
        "key": "alt+cmd+backspace",
        "command": "-deleteFile",
        "when": "explorerViewletVisible && filesExplorerFocus"
    }
]
```

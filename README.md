# VS Code Settings

# Font

* [Meslo Font](https://github.com/fontmgr/MesloLGSNF)

## Themes/Color

* [Just Black]()
  * See [`editor.tokenColorCustomizations`](#settings) in my VS Code settings for a rew modifications I make to the theme.

## Extensions

* Theme / Editor Experience

  * [FontSize ShortCuts]()
    * Change the font size with keyboard shortcuts.
  * [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons)
    * Nice / colorful icons for many different file types
  * [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
    * Integrates ESLint JS
  * [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
    * Automatically format javascript, JSON, CSS, Sass

* Languages and Libraries
  * [Auto Close Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag)
    * Automatically add HTML/XML close tag
  * [Auto Import](https://marketplace.visualstudio.com/items?itemName=steoates.autoimport)
    * Automatically finds, parses and provides code actions and code completion for all available imports. Works with Typescript and TSX
  * [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
    * Auto rename paired HTML/XML tag
  * [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)
    * View a Git Graph of your repository, and perform Git actions from the graph.
  * [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
    * Visual Studio Code plugin that autocompletes filenames
  * [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)
    * Intelligent Tailwind CSS tooling for VS Code.

* React
  * [ES7+ React/Redux/React-Native snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)
    * Extensions for React, React-Native and Redux in JS/TS with ES7+ syntax. Customizable. Built-in integration with prettier.
  * [Prisma](https://marketplace.visualstudio.com/items?itemName=Prisma.prisma)
    * Adds syntax highlighting, formatting, auto-completion, jump-to-definition and linting for .prisma files.

### Extension package names for easy install

# Settings

```json
{
  // editor
  "diffEditor.wordWrap": "on", // on: Wiersze będą zawijane przy szerokości okienka ekranu.
  "editor.detectIndentation": false, // Określa, czy #editor.tabSize# i #editor.insertSpaces# będą automatycznie wykrywane po otwarciu pliku na podstawie zawartości pliku.
  "editor.fontFamily": "MesloLGS Nerd Font",
  "editor.fontLigatures": true,
  "editor.fontSize": 14,
  "editor.letterSpacing": 0.2,
  "editor.mouseWheelZoom": true, // command + kółko myszki.
  "editor.wordWrap": "on", // zawijanie wierszy dostosowane do aktualnej szerokości okna
  "editor.formatOnPaste": false,
  "editor.inlineSuggest.enabled": true, // Określa, czy automatycznie wyświetlać wbudowane sugestie w edytorze.
  "editor.lineHeight": 1.6,
  "editor.linkedEditing": true, //Określa, czy w edytorze jest włączone edytowanie połączone. Zależnie od języka, powiązane symbole (np. tagi HTML) są aktualizowane podczas edytowania.
  "editor.minimap.enabled": false,
  "editor.multiCursorModifier": "ctrlCmd", // ctrlCmd: Mapuje na klawisz „Control” na klawisz „Command” w systemie macOS.
  "editor.snippetSuggestions": "top",
  "editor.suggestSelection": "first", // Określa sposób wstępnego wybierania sugestii podczas wyświetlania listy sugestii. first: Zawsze wybieraj pierwszą sugestię.
  "editor.tabSize": 2,
  "editor.unicodeHighlight.invisibleCharacters": false, // Określa, czy znaki, które tylko rezerwują miejsce lub nie mają żadnej szerokości, są wyróżniane.
  // emmet
  "emmet.showAbbreviationSuggestions": false, // Pokazuje możliwe skróty wtyczki Emmet jako sugestie. Nie dotyczy arkuszy stylów lub gdy właściwość emmet.showExpandedAbbreviation ma wartość „never”.
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "typescript": "typescriptreact"
  },
  // eslint
  "eslint.enable": true,
  "eslint.validate": [
    // Tablica języtków, które będą sprawdzane przez Eslint. Jeżeli ESLint nie jest zainstalowany, wyświetli błąd.
    "react",
    "typescript",
    "html",
    "javascript"
  ],
  // explorer
  "explorer.openEditors.visible": 1, // Początkowa liczba pokazanych plików w edycji. Jeeli będzie ich więcej zostanie wyświetlony pasek przewijania.
  "explorer.compactFolders": false,
  // extensions
  "extensions.ignoreRecommendations": true, // Powiadomienia o rekomendacjach dotyczących rozszerzeń nie będą wyświetlane.
  // files
  "files.autoSave": "onWindowChange", // onWindowChange: Edytor zawierający zmiany jest automatycznie zapisywany, gdy okno utraci fokus.
  "files.eol": "\n",
  "files.trimTrailingWhitespace": true,
  "files.trimFinalNewlines": true,
  "files.insertFinalNewline": true,
  //git
  "git.autofetch": true, // W przypadku ustawienia wartości true zatwierdzenia będą automatycznie pobierane z domyślnego repozytorium zdalnego bieżącego repozytorium Git.
  "git.openRepositoryInParentFolders": "never", // never: Nigdy nie otwieraj repozytorium w folderach nadrzędnych obszarów roboczych lub otwartych plików.
  // markdown
  "markdown.preview.fontSize": 12,
  "screencastMode.keyboardOptions": {
    // Opcje dostosowywania nakładki klawiatury w trybie rzutowania ekranu.
    "showKeys": true,
    "showKeybindings": true,
    "showCommands": true,
    "showCommandGroups": false,
    "showSingleEditorCursorMoves": true
  },
  // search
  "search.exclude": {
    // Wykluczenie katalogów w procesie wyszukiwania
    "**/node_modules": true,
    "**/bower_components": true,
    "**/*.code-search": true
  },
  "search.useIgnoreFiles": false, // Określa, czy podczas wyszukiwania plików używać plików „.gitignore” i „.ignore”.
  // terminal
  "terminal.integrated.fontSize": 14,
  //vsicons
  "vsicons.dontShowNewVersionMessage": true,
  // window
  "window.zoomLevel": 1, // powiększenie o 20%
  "window.title": "${activeEditorMedium}${separator}${rootName}",
  // workbench
  "workbench.colorTheme": "Default Dark+",
  "workbench.editor.labelFormat": "medium", // medium: Pokaż nazwę pliku, po której następuje jego ścieżka względem folderu obszaru roboczego.
  "workbench.editor.showTabs": "none", // none: Obszar tytułu edytora nie jest wyświetlany.
  "workbench.iconTheme": "vscode-icons",
  "workbench.sideBar.location": "right",
  "workbench.startupEditor": "newUntitledFile", // newUntitledFile: Otwórz nowy plik bez tytułu (ma zastosowanie tylko przy otwieraniu pustego okna).
  "workbench.statusBar.visible": true,
  "workbench.colorCustomizations": {
    "titleBar.activeForeground": "#000",
    "titleBar.inactiveForeground": "#000000CC",
    "titleBar.activeBackground": "#FFC600",
    "titleBar.inactiveBackground": "#FFC600CC",
    "window.activeBorder": "#00FFFF",
    "window.inactiveBorder": "#FF0000"
  },
  // formatowanie plików
  "[css]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[json]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[markdown]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[scss]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  }
}
```

# Keybindings

```json
[
  {
    "key": "cmd+1",
    "command": "workbench.action.openEditorAtIndex1"
  },
  {
    "key": "cmd+2",
    "command": "workbench.action.openEditorAtIndex2"
  },
  {
    "key": "cmd+3",
    "command": "workbench.action.openEditorAtIndex3"
  },
  {
    "key": "cmd+4",
    "command": "workbench.action.openEditorAtIndex4"
  },
  {
    "key": "cmd+5",
    "command": "workbench.action.openEditorAtIndex5"
  },
  {
    "key": "cmd+6",
    "command": "workbench.action.openEditorAtIndex6"
  },
  {
    "key": "cmd+7",
    "command": "workbench.action.openEditorAtIndex7"
  },
  {
    "key": "cmd+8",
    "command": "workbench.action.openEditorAtIndex8"
  },
  {
    "key": "cmd+9",
    "command": "workbench.action.openEditorAtIndex9"
  }
]
```

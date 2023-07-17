### Экспорт расширений
```
code --list-extensions | xargs -L 1 echo code --install-extension
```

### Расширения
```
code --install-extension akamud.vscode-theme-onedark
code --install-extension alexcvzz.vscode-sqlite
code --install-extension Atishay-Jain.All-Autocomplete
code --install-extension batisteo.vscode-django
code --install-extension bibhasdn.django-snippets
code --install-extension bigonesystems.django
code --install-extension burkeholland.simple-react-snippets
code --install-extension christian-kohler.path-intellisense
code --install-extension donjayamanne.githistory
code --install-extension donjayamanne.jquerysnippets
code --install-extension donjayamanne.python-environment-manager
code --install-extension donjayamanne.python-extension-pack
code --install-extension dsznajder.es7-react-js-snippets
code --install-extension ecmel.vscode-html-css
code --install-extension Equinusocio.vsc-material-theme
code --install-extension equinusocio.vsc-material-theme-icons
code --install-extension esbenp.prettier-vscode
code --install-extension FallenMax.mithril-emmet
code --install-extension formulahendry.auto-rename-tag
code --install-extension glenn2223.live-sass
code --install-extension GrapeCity.gc-excelviewer
code --install-extension HookyQR.beautify
code --install-extension ionutvmi.path-autocomplete
code --install-extension KevinRose.vsc-python-indent
code --install-extension mhutchie.git-graph
code --install-extension michelemelluso.gitignore
code --install-extension mrcrowl.easy-less
code --install-extension mrmlnc.vscode-less
code --install-extension mrmlnc.vscode-scss
code --install-extension MS-CEINTL.vscode-language-pack-ru
code --install-extension ms-dotnettools.csharp
code --install-extension ms-python.black-formatter
code --install-extension ms-python.isort
code --install-extension ms-python.python
code --install-extension ms-python.vscode-pylance
code --install-extension ms-vscode.cmake-tools
code --install-extension ms-vscode.cpptools
code --install-extension ms-vscode.cpptools-extension-pack
code --install-extension ms-vscode.cpptools-themes
code --install-extension ms-vscode.vscode-typescript-next
code --install-extension njpwerner.autodocstring
code --install-extension PKief.material-icon-theme
code --install-extension platformio.platformio-ide
code --install-extension pmneo.tsimporter
code --install-extension pranaygp.vscode-css-peek
code --install-extension ritwickdey.LiveServer
code --install-extension samuelcolvin.jinjahtml
code --install-extension skyran.js-jsx-snippets
code --install-extension streetsidesoftware.code-spell-checker
code --install-extension streetsidesoftware.code-spell-checker-russian
code --install-extension twxs.cmake
code --install-extension VisualStudioExptTeam.intellicode-api-usage-examples
code --install-extension VisualStudioExptTeam.vscodeintellicode
code --install-extension wayou.vscode-todo-highlight
code --install-extension wholroyd.jinja
code --install-extension xabikos.JavaScriptSnippets
code --install-extension yzhang.markdown-all-in-one
code --install-extension zhoufeng.pyqt-integration
code --install-extension zhuangtongfa.material-theme
code --install-extension Zignd.html-css-class-completion
```

### Настройки:

```
{
    "telemetry.enableTelemetry": false,
    "editor.wordWrap": "wordWrapColumn",
    "git.enableSmartCommit": true,
    "git.confirmSync": false,
    "editor.linkedEditing": true,
    "git.autofetch": true,
    "liveServer.settings.donotShowInfoMsg": true,
    "workbench.startupEditor": "none",
    "workbench.iconTheme": "material-icon-theme",
    "files.associations": {
        "**/*.html": "html",
        "**/templates/**/*.html": "django-html",
        "**/requirements{/**,*}.{txt,in}": "pip-requirements"
    },
    "security.workspace.trust.untrustedFiles": "open",
    "explorer.confirmDelete": false,
    "files.autoSave": "afterDelay",
    "editor.mouseWheelZoom": true,
    "workbench.editorAssociations": {
        "*.docx": "default"
    },
    "settingsSync.ignoredSettings": ["-window.zoomLevel"],
    "[python]": {
        "editor.formatOnSave": false,
        "editor.defaultFormatter": "ms-python.black-formatter"
    },
    "python.formatting.provider": "black",
    "liveServer.settings.donotVerifyTags": true,
    "cmake.configureOnOpen": false,
    "workbench.preferredDarkColorTheme": "Atom One Dark",
    "editor.wordWrapColumn": 160,
    "editor.fontFamily": "Fira Code, Menlo, Monaco, 'Courier New', monospace",
    "editor.fontLigatures": true,
    "editor.lineHeight": 1.6,
    "[jsonc]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "prettier.printWidth": 160,
    "prettier.tabWidth": 4,
    "git-graph.dialog.addTag.pushToRemote": true,
    "git-graph.commitDetailsView.location": "Docked to Bottom",
    "files.exclude": {
        "**/__pycache__": true,
        "**/.idea": true,
        "**/.vscode": true
    },
    "window.zoomLevel": 1,
    "keyboard.dispatch": "keyCode",
    "editor.fontSize": 13,
    "emmet.includeLanguages": {
        "django-html": "html",
        "jinja-html": "html",
        "javascript": "javascriptreact"
    },
    "python.linting.pylintEnabled": true,
    "python.linting.pylintArgs": ["--load-plugins", "pylint_django", "--django-settings-module=core.settings", "--max-line-length=120"],
    "python.formatting.blackArgs": ["--line-length=120"],
    "[html]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "prettier.useTabs": true,
    "reactSnippets.settings.prettierEnabled": true,
    "beautify.language": {
        "html": [
            "htm",
            "html",
            "django-html"
        ]
    },
    "[django-html]": {
        "editor.defaultFormatter": "HookyQR.beautify"
    },
    "auto-rename-tag.activationOnLanguage": [
        "html",
        "xml",
        "php",
        "javascript",
        "django-html"
    ],
    "[css]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "cSpell.language": "en,ru",
    "workbench.colorTheme": "One Dark Pro",
    "path-intellisense.autoSlashAfterDirectory": true,
    "path-intellisense.autoTriggerNextSuggestion": true,
    "path-intellisense.showHiddenFiles": true,
    "[javascript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "cSpell.userWords": [
        "Дебаггер",
        "bootloader",
        "netsh",
        "nmcli",
        "ssid",
        "ssids",
        "venv",
        "wlan"
    ],
}
```
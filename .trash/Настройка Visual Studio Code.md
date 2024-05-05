### Экспорт расширений
```bash
code --list-extensions | xargs -L 1 echo code --install-extension
```

### Расширения
```
code --install-extension akamud.vscode-theme-onedark
code --install-extension alexcvzz.vscode-sqlite
code --install-extension atishay-jain.all-autocomplete
code --install-extension batisteo.vscode-django
code --install-extension bibhasdn.django-snippets
code --install-extension bigonesystems.django
code --install-extension burkeholland.simple-react-snippets
code --install-extension christian-kohler.npm-intellisense
code --install-extension christian-kohler.path-intellisense
code --install-extension codezombiech.gitignore
code --install-extension davidanson.vscode-markdownlint
code --install-extension dbaeumer.vscode-eslint
code --install-extension donjayamanne.githistory
code --install-extension donjayamanne.jquerysnippets
code --install-extension donjayamanne.python-environment-manager
code --install-extension donjayamanne.python-extension-pack
code --install-extension dotjoshjohnson.xml
code --install-extension dsznajder.es7-react-js-snippets
code --install-extension ecmel.vscode-html-css
code --install-extension editorconfig.editorconfig
code --install-extension equinusocio.vsc-material-theme
code --install-extension equinusocio.vsc-material-theme-icons
code --install-extension esbenp.prettier-vscode
code --install-extension fallenmax.mithril-emmet
code --install-extension formulahendry.auto-close-tag
code --install-extension formulahendry.auto-rename-tag
code --install-extension formulahendry.code-runner
code --install-extension github.github-vscode-theme
code --install-extension glenn2223.live-sass
code --install-extension golang.go
code --install-extension grapecity.gc-excelviewer
code --install-extension hediet.vscode-drawio
code --install-extension ionutvmi.path-autocomplete
code --install-extension kevinrose.vsc-python-indent
code --install-extension mechatroner.rainbow-csv
code --install-extension mrmlnc.vscode-scss
code --install-extension ms-ceintl.vscode-language-pack-ru
code --install-extension ms-python.black-formatter
code --install-extension ms-python.debugpy
code --install-extension ms-python.isort
code --install-extension ms-python.pylint
code --install-extension ms-python.python
code --install-extension ms-python.vscode-pylance
code --install-extension ms-vscode.cmake-tools
code --install-extension ms-vscode.cpptools
code --install-extension ms-vscode.cpptools-extension-pack
code --install-extension ms-vscode.cpptools-themes
code --install-extension ms-vscode.makefile-tools
code --install-extension ms-vscode.vscode-typescript-next
code --install-extension msjsdiag.vscode-react-native
code --install-extension njpwerner.autodocstring
code --install-extension njqdev.vscode-python-typehint
code --install-extension oderwat.indent-rainbow
code --install-extension pkief.material-icon-theme
code --install-extension pkief.material-product-icons
code --install-extension pmneo.tsimporter
code --install-extension pranaygp.vscode-css-peek
code --install-extension redhat.vscode-xml
code --install-extension ritwickdey.liveserver
code --install-extension samuelcolvin.jinjahtml
code --install-extension skyran.js-jsx-snippets
code --install-extension streetsidesoftware.code-spell-checker
code --install-extension streetsidesoftware.code-spell-checker-russian
code --install-extension styled-components.vscode-styled-components
code --install-extension tabnine.tabnine-vscode
code --install-extension tomoki1207.pdf
code --install-extension twxs.cmake
code --install-extension usernamehw.errorlens
code --install-extension visualstudioexptteam.intellicode-api-usage-examples
code --install-extension visualstudioexptteam.vscodeintellicode
code --install-extension vscode-icons-team.vscode-icons
code --install-extension wayou.vscode-todo-highlight
code --install-extension wholroyd.jinja
code --install-extension xabikos.javascriptsnippets
code --install-extension yzhang.markdown-all-in-one
code --install-extension zhoufeng.pyqt-integration
code --install-extension zhuangtongfa.material-theme
code --install-extension zignd.html-css-class-completion
```

### Настройки:

```json
{
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
	"[python]": {
		"editor.formatOnSave": true,
		"editor.defaultFormatter": "ms-python.black-formatter"
	},
	"liveServer.settings.donotVerifyTags": true,
	"cmake.configureOnOpen": false,
	"editor.wordWrapColumn": 160,
	"editor.fontFamily": "Fira Code, Menlo, Monaco, 'Courier New', monospace",
	"editor.fontLigatures": true,
	"editor.lineHeight": 1.6,
	"[jsonc]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode"
	},
	"prettier.tabWidth": 4,
	"files.exclude": {
		"**/__pycache__": true,
		"**/.idea": true,
		"**/.vscode": true
	},
	"emmet.includeLanguages": {
		"django-html": "html",
		"jinja-html": "html",
		"javascript": "javascriptreact"
	},
	"[html]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode"
	},
	"prettier.useTabs": true,
	"reactSnippets.settings.prettierEnabled": true,
	"auto-rename-tag.activationOnLanguage": ["html", "xml", "php", "javascript", "django-html"],
	"[css]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode"
	},
	"cSpell.language": "en,ru",
	"workbench.colorTheme": "GitHub Dark",
	"path-intellisense.autoSlashAfterDirectory": true,
	"path-intellisense.autoTriggerNextSuggestion": true,
	"path-intellisense.showHiddenFiles": true,
	"[javascript]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode"
	},
	"cSpell.userWords": [
		"Дебаггер",
		"нацпроекту",
		"недостроя",
		"Парсер",
		"парсить",
		"УМВД",
		"эндпоинт",
		"antd",
		"apexcharts",
		"bootloader",
		"consts",
		"DATEONLY",
		"Datepicker",
		"dotenv",
		"echarts",
		"EDMS",
		"freqs",
		"fuzzywuzzy",
		"fyne",
		"gitea",
		"Hovedplan",
		"iefix",
		"iframes",
		"jivo",
		"lxml",
		"netsh",
		"nmcli",
		"novyigorod",
		"openpyxl",
		"perz",
		"Pixmap",
		"Pressable",
		"pylint",
		"reduxjs",
		"sheetnames",
		"Sider",
		"ssid",
		"ssids",
		"venv",
		"wlan",
		"Wremena"
	],
	"cmake.showOptionsMovedNotification": false,
	"indentRainbow.indicatorStyle": "light",
	"debug.enableStatusBarColor": false,
	"[typescriptreact]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode"
	},
	"[typescript]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode"
	},
	"[scss]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode"
	},
	"editor.formatOnSave": true,
	"prettier.printWidth": 120,
	"python.envFile": "${workspaceFolder}/.venv",
	"pylint.args": [
		"--max-line-length=120",
		"--disable=C0114",
		"--disable=C0115",
		"--disable=C0116",
		"--extension-pkg-whitelist=PyQt5,PyQt6"
	],
	"python.languageServer": "Pylance",
	"python.venvFolders": ["venv", ".venv"],
	"workbench.productIconTheme": "material-product-icons",
	"telemetry.telemetryLevel": "off",
	"window.restoreWindows": "none",
	"files.hotExit": "off",
	"[markdown]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode"
	},
	"go.toolsManagement.autoUpdate": true,
	"pyqt-integration.qtdesigner.path": ".venv\\Lib\\site-packages\\qt6_applications\\Qt\\bin\\designer.exe",
	"tabnine.experimentalAutoImports": true,
	"[json]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode"
	},
	"pyqt-integration.pyuic.compile.filepath": "./${ui_name}.py",
	"[xml]": {
		"editor.defaultFormatter": "redhat.vscode-xml"
	},
	"hediet.vscode-drawio.resizeImages": null,
	"pyqt-integration.pyuic.cmd": "pyuic6",
	"[javascriptreact]": {
		"editor.defaultFormatter": "esbenp.prettier-vscode"
	}
}
```
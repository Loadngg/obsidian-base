## `Lazy` - менеджер плагинов:
#### Его вызов:
```
:Lazy
```

Есть 2 варианта установки нового плагина:
1. Если на странице плагина на `GitHub` есть пункт установки для `Lazy`, то копируем и вставляем. Например:
```
require("lazy").setup({
	{
		"folke/tokyonight.nvim",
		lazy = false,
		priority = 1000,
		opts = {},
	},
})
```
2. Иначе тупо вставляем ссылку на `GitHub` плагина
```
require("lazy").setup({
	{ "joshdick/onedark.vim" },
})
```


## `Treesitter` - улучшенная подсветка синтаксиса:
#### Новые языки устанавливаются при помощи добавления в `ensure_installed` и команды:
```
:TSInstall язык
```

## `Lsl` - языковые серверы:
#### Новые сервера конфигурируются так:
```
lspconfig.pyright.setup({})
```

## `Nul-ls` - конфигурация диагностики и форматирования:
Пример:

```
...

null_ls.setup({
	sources = {
		null_ls.builtins.formatting.stylua,
		null_ls.builtins.diagnostics.standardjs,
		null_ls.builtins.formatting.prettierd.with({
			cli_options = {
				single_quote = true,
				print_width = 80,
				semi = false,
				tab_width = 4,
				use_tabs = true,
			},
			filetypes = {
				"css",
				"scss",
				"less",
				"json",
				"jsonc",
				"yaml",
				"markdown",
				"markdown.mdx",
				"graphql",
				"handlebars",
			},
		}),
	},
	...
}
```

## [[Mason]] - менеджер пакетов:
####  Его вызов:
```
:Mason
```

## [[Конфиги prettier, eslint и stylelint]]

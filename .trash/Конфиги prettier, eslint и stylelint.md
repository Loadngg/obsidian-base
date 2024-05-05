### Prettier
`.prettierrc.json`:
```json
{
	"printWidth": 80,
	"tabWidth": 4,
	"useTabs": false,
	"semi": false,
	"singleQuote": false,
	"quoteProps": "as-needed",
	"jsxSingleQuote": false,
	"trailingComma": "es5",
	"bracketSpacing": true,
	"bracketSameLine": false,
	"arrowParens": "always",
	"endOfLine": "lf"
}
```

`.prettierignore`:
```
dist
coverage

*.yaml
```

### Eslint
`.eslintrc.js`:
```js
module.exports = {
    env: {
        browser: true,
        es2021: true,
    },
    extends: ["eslint:recommended"],
    parserOptions: {
        ecmaVersion: "latest",
        sourceType: "module",
    },
    rules: {},
}
```

`.eslintiognore`:
```
dist
coverage
*.yaml
.eslintrc.js
```

### Stylelint
`.stylelintrc.json`:
```json
{
	"rules": {
		"selector-class-pattern": [
			"^([a-z][a-z]+)+(__([a-z][a-z]+)+)?(_[a-z]+([a-z][a-z]+)*){0,2}$",
			{
				"message": "Selector class pattern does not match project conventions",
				"resolveNestedSelectors": true
			}
		]
	}
}
```

`.stylelintignore`:
```
node_modules
bin
*.*
!*.css
!*.scss
```

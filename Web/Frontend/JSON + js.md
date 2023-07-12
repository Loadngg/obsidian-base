Тестовый файл `config.json`:
```
{
    "backend_url": "http://localhost:5115/"
}
```

Функция получения файла `config.json`:
```
getConfig: () => {
	try {
		const request = new XMLHttpRequest();
		request.open("GET", "{путь до файла}/{файл}.json", false);
		request.send(null)
		return JSON.parse(request.responseText)
	} catch (e) {
		window.alert("Не найден файл конфигурации.")
	}
}
```

Пример использования:
```
const CONFIG = utils.getConfig();
export const BACKEND = CONFIG.backend_url
const BACKEND_USER = `${BACKEND}user/`
```
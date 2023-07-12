Пример `Makefile`:
```
run:
	docker run -d -p 80:4200 --env-file ./config/.env --rm --name testapp testapp:latest

stop:
	docker stop testapp
```
Пример `dockerfile`:
```dockerfile
FROM node

WORKDIR /app

COPY . .

RUN npm install

ENV PORT 3000

EXPOSE $PORT

CMD [ "node" , "App.js"]

```

`FROM` - Образ, на основе которого будет основан новый образ приложения

`WORKDIR` - папка, где будет храниться `image` приложения

`ENV` - переменные окружения
Синтаксис:
```
PORT [название переменной] [её значение]
```

`COPY` - копировать файлы
Синтаксис:
```
COPY [папка, откуда копировать] [папка, куда копировать]
```

`RUN` - запуск команды единожды при создании image

`EXPOSE` - на каком порте будет запущен контейнер (не обязательно, но считается хорошей практикой)

`CMD` - команда для запуска в виде массива слов

# Использование
Нужно установить библиотеку в ту папку где находится код и импортировать эту библиотеку
```javascript
import paper
```
Ссылка для скачивания библиотеки:
```javascript
https://drive.google.com/file/d/14CnVBRZYI1T18MRiTBToIj3Idku7MsC9/view?usp=drivesdk
```

# send
Осуществляет перевод другому пользователю

Включает в себя 3 параметра:
```
api_token ```- обязательный - ваш токен (str)

to - обязательный - кому перевести (int)

summa - обязательный - сумма перевода (int)

Пример использования:
```javascript
send = paper.send("TOKEN", 1, 100)
print(send)
```

# getLink
Возвращает ссылку для перевода

Включает в себя 2 параметра:

id - обязательный - для кого создается ссылка (int)

summa - обязательный - сумма перевода (int)

Пример использования:
```javascript
link = paper.getLink(1, 100)
print(link)
```

# score
Возвращает баланс пользователя

Включает в себя 2 параметра:

api_token - обязательный - ваш токен (str)

id - обязательный - чей баланс узнать (int)

Пример использования:
```javascript
balance = paper.score("TOKEN", 1)
print(balance)
```

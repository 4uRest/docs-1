## userLogin: авторизация пользователя

```javascript
Poster.on('userLogin', (res) => {
	console.log(res);
})
```

Событие срабатывает после входа пользователя на терминал. Например, после ввода PIN кода или при быстрой смене официанта. 

### Ответ

В качестве аргумента в обработчик приходит объект `data` с такими свойствами

Свойство | Значение
-------- | --------
user | Сотрудник который вошел на терминал, объект типа [User](/docs/v3/pos/types/user) 

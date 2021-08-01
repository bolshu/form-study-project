# Form study project

## Макет
```
https://www.figma.com/file/oEox18VbeVdWPifGqj5PbK/Form-study-project?node-id=0%3A1
```

## Техническое задание

1. Сверстать форму
1. При ответе с сервера под заголовком формы появляется нотис с состоянием ответа с сервера (см. макет). Текст сообщения приходит с сервера
1. Нотис можно убрать при клике на крестик (см. макет)
1. После успешной отправки формы поля формы очищаются. Если сервер отдает ошибку, то поля не очищаются

## Запуск и разработка

### Установить зависимости
```
npm install
```

### Запустить сервер

Сервер запускается на порту `3000`: `http://localhost:3000/`

```
npm run start
```

## API

### Тело запроса

```
{
  name: string;
  email: string;
  phone: string;
}
 ```

 Одно из полей `email` и `phone` является обязательным.

### Коды ответов

`200` — success

`400` — fail. Когда не передали одно из полей `email` или `phone`

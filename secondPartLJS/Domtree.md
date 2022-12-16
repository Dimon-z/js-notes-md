Основа html документа  это теги
в соответствии с DOM каждый тег это обьект теги внутри являются дочерними для тега верхнего уровня. Любое содержимое тега так же является дочерним обьектом 
Все эти обьекты доступны из JS. Мы можем использовать их для изменения страницы.
```javascript
document.body.style.background = 'red'; // сделать фон красным

setTimeout(() => document.body.style.background = '', 3000); // вернуть назад
```


Начнём с такого, простого, документа:

```markup
<!DOCTYPE HTML>
<html>
<head>
  <title>О лосях</title>
</head>
<body>
  Правда о лосях.
</body>
</html>
```

DOM – это представление HTML-документа в виде дерева тегов. Вот как оно выглядит:


![alt text](https://github.com/Dimon-z/js-notes-md/blob/develop/assets/bmp/DomProst.bmp?raw=true)

каждый узел дерева - обьект. У тектовых узлов не бывает потомков.

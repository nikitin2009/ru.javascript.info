
# Загрузить массив последовательно

Есть массив URL:

```js run
'use strict';

let urls = [
  'user.json',
  'guest.json'
];
```

Напишите код, который все URL из этого массива загружает один за другим (последовательно) и сохраняет результаты в массиве `results`, а потом выводит.

Вариант с параллельной загрузкой выглядел бы так:

```js
Promise.all( urls.map(httpGet) )
  .then(alert);
```

В этой задаче загрузку нужно реализовать последовательно.


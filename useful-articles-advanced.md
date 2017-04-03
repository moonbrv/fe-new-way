# Полезные статейки по JS [03.04.2017]

## [Кратко о том что вообще происходит в мире js, обзор терминов и понятий](https://medium.com/devschacht/glossary-of-modern-javascript-concepts-1198b24e8f56)

## Иммутабельность
О том что это, зачем нужо и какие в этом выгоды описано в [этом ответе на stackowerflow](http://stackoverflow.com/questions/34385243/why-is-immutability-so-importantor-needed-in-javascript), а так же даны несколько интересных ссылок на эту тему.
Парочку примеров использования принципа иммутабельности в ES6 [можно посмотереть тут](https://wecodetheweb.com/2016/02/12/immutable-javascript-using-es6-and-beyond/).

## ES6
Для тех кто слабо знаком рекомендую статьи на [jsracoon](http://jsraccoon.ru/tag/es6), читать начиная с последней, если что.
Я бы к этому добавил еще:
```javascript
/* Создание масива из колекции элементов*/
Array.of(document.querySelectorAll('.className'))

/* Иммутабельное изменение/присваивание объекта */
let oldObj = {
  a: 10,
  b: 'hohoho'
}
oldObj = Object.assign({}, oldObj, {a: 20})
console.log(oldObj)
// {a: 20, b: 'hohoho'}
```
Вот впринципе и все что нужно обязательно знать...
Краткий справочник о новый возможностях можно [посмотреть тут](http://babeljs.io/learn-es2015/). На ютубе полно видео уроков, вот [хорошие туторы на русском](https://www.youtube.com/watch?v=4YfsAz-sNAo&list=PLqHlAwsJRxAOpWPtj2T6HhSzX-lKmKV2q).

Вот еще хороший [цикл статей, в блоге умного дядьки](https://ponyfoo.com/books/practical-es6/chapters#toc).


## Функциональное програмирование
А теперь во все тяжкие...

Нужно очень хорошо понимать что такое функции высшего порядка - лучший ответ на этот вопрос с неплохим поясняющим видосиком [можно найти тут](https://www.quora.com/What-is-a-simple-explanation-of-higher-order-functions-and-callbacks-in-JavaScript).

Большинство всяких хитрожопых функций уже написано до нас:
 - [Lodash](https://lodash.com/)
 - [Ramda](http://ramdajs.com)

 Только не забывайте импортировать функции оттуда как отдельные модули, нету смысла тянуть всю библиотеку.

Жаргон функционального програмирования ([Eng](https://github.com/hemanth/functional-programming-jargon) / [Rus](https://habrahabr.ru/post/310172/))

Книги по ФП в js:
- [Хорошая книга на эту тему №1](https://github.com/getify/Functional-Light-JS#book)
- [Хорошая книга на эту тему №2](https://github.com/MostlyAdequate/mostly-adequate-guide)

Будет дополнятся...
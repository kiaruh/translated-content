---
title: 'SyntaxError: missing name after . operator(отсутствует имя после. оператора)'
slug: Web/JavaScript/Reference/Errors/Missing_name_after_dot_operator
translation_of: Web/JavaScript/Reference/Errors/Missing_name_after_dot_operator
---
{{jsSidebar("Errors")}}

## Сообщение

```
SyntaxError: missing name after . operator
```

## Тип ошибки

{{jsxref("SyntaxError")}}

## Что пошло не так?

Оператор точки (.) используется для доступа к свойству. Необходимо указать имя свойства, к которому требуется получить доступ. Для доступа к вычисляемому свойству может потребоваться изменить доступ к свойству с точки на квадратные скобки. Это позволит вычислить выражение. Может быть, вы собирались сделать конкатенацию вместо этого? В этом случае необходим оператор plus ( + ). См. примеры ниже.

## Примеры

### Доступ к свойствам

Методы доступа к свойствам в JavaScript используют точку (.) или квадратные скобки (\[]), но не оба. Квадратные скобки обеспечивают доступ к вычисляемым свойствам.

```js example-bad
var obj = { foo: { bar: "baz", bar2: "baz2" } };
var i = 2;

obj.[foo].[bar]
// SyntaxError: отсутствует имя после оператора .

obj.foo."bar"+i;
// SyntaxError: отсутствует имя после оператора .
```

Чтобы исправить этот код, необходимо получить доступ к объекту следующим образом:

```js example-good
obj.foo.bar; // "baz"
//или же
obj["foo"]["bar"]; // "baz"

//вычисляемые свойства требуют квадратных скобок
obj.foo["bar" + i]; // "baz2"
```

### Доступ к свойствам против конкатенации

Если вы пришли из другого языка программирования (например, {{Glossary("PHP")}}), также легко перепутать оператор точки (.) и оператор конкатенации (+).

```js example-bad
console.log("Hello" . "world");

// SyntaxError: missing name after . operator
```

Вместо этого необходимо использовать знак плюс для объединения:

```js example-good
console.log("Hello" + "World");
```

## Смотрите также

- [Property accessors](/ru/docs/Web/JavaScript/Reference/Operators/Property_Accessors)(доступ к свойствам)

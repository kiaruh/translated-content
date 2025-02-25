---
title: Math.sin()
slug: Web/JavaScript/Reference/Global_Objects/Math/sin
tags:
  - JavaScript
  - Math
  - Method
  - Reference
translation_of: Web/JavaScript/Reference/Global_Objects/Math/sin
---
{{JSRef("Global_Objects", "Math")}}

## Сводка

Метод **`Math.sin()`** возвращает синус числа.

## Синтаксис

```
Math.sin(x)
```

### Параметры

- `x`
  - : Число радиан.

## Описание

Метод `Math.sin()` возвращает числовое значение от -1 до 1, которое представляет синус переданного (в радианах) угла.

Поскольку метод `sin()` является статическим методом объекта `Math`, вы всегда должны использовать его как `Math.sin()`, а не пытаться вызывать метод на созданном экземпляре объекта `Math` (поскольку объект `Math` не является конструктором).

## Примеры

### Пример: использование метода `Math.sin()`

```js
Math.sin(0);           // 0
Math.sin(1);           // 0.8414709848078965

Math.sin(Math.PI / 2); // 1
```

## Спецификации

| Спецификация                                                         | Статус                   | Комментарии                                            |
| -------------------------------------------------------------------- | ------------------------ | ------------------------------------------------------ |
| ECMAScript 1-е издание.                                              | {{Spec2('ES1')}}     | Изначальное определение. Реализована в JavaScript 1.0. |
| {{SpecName('ES5.1', '#sec-15.8.2.16', 'Math.sin')}} | {{Spec2('ES5.1')}} |                                                        |
| {{SpecName('ES6', '#sec-math.sin', 'Math.sin')}}     | {{Spec2('ES6')}}     |                                                        |

## Совместимость с браузерами

{{Compat}}

## Смотрите также

- {{jsxref("Math.acos()")}}
- {{jsxref("Math.asin()")}}
- {{jsxref("Math.atan()")}}
- {{jsxref("Math.atan2()")}}
- {{jsxref("Math.cos()")}}
- {{jsxref("Math.tan()")}}

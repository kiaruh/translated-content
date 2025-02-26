---
title: HTMLHyperlinkElementUtils.port
slug: Web/API/HTMLAnchorElement/port
tags:
  - API
  - Experimental
  - HTMLHyperlinkElementUtils
  - Property
  - URL API
translation_of: Web/API/HTMLHyperlinkElementUtils/port
original_slug: Web/API/HTMLHyperlinkElementUtils/port
---
{{ApiRef("URL API")}}

Свойство **`HTMLHyperlinkElementUtils.port`** – это {{domxref("USVString")}}, содержащий номер порта.

При значении `'' будет использоваться` порт по умолчанию для указанного протокола (не `0`).

## Синтаксис

```
string = object.port;
object.port = string;
```

## Примеры

```js
// Допустим, что документ содержит элемент <a id="myAnchor" href="https://developer.mozilla.org/en-US/docs/HTMLHyperlinkElementUtils.port">
var anchor = document.getElementByID("myAnchor");
var result = anchor.port; // Вернёт: '80'
```

## Спецификации

{{Specifications}}

## Совместимость с браузерами

{{Compat}}

## Смотрите также

- Миксин {{domxref("HTMLHyperlinkElementUtils")}}, к которому принадлежит это свойство.

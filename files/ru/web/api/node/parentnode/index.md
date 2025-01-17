---
title: Node.parentNode
slug: Web/API/Node/parentNode
tags:
  - API
  - DOM
  - Method
translation_of: Web/API/Node/parentNode
---
{{ApiRef}}

## Аннотация

Возвращает родителя определённого элемента DOM дерева.

## Синтаксис

```
parentNode = node.parentNode
```

`parentNode` родитель текущего элемента. Родитель элемента является `Element` узлом, `Document` узлом, или `DocumentFragment` узлом.

## Пример

```js
if (node.parentNode) {
  // удаляем элемент из дерева
  node.parentNode.removeChild(node);
}
```

## Примечание

`Document` и `DocumentFragment` [nodes](/ru/docs/DOM/Node.nodeType "DOM/Node.nodeType") _могут не иметь родителя_, в этом случае `parentNode` всегда возвращает `null`.

Так же возвращает `null` если элемент только был создан и ещё не добавлен в DOM дерево.

## Поддержка браузерами

{{Compat}}

## Спецификация

- [DOM Level 2 Core: Node.parentNode](http://www.w3.org/TR/DOM-Level-2-Core/core.html#ID-1060184317)
- [DOM Level 3 Core: Node.parentNode](http://www.w3.org/TR/DOM-Level-3-Core/core.html#ID-1060184317)

## Смотрите также

- {{Domxref("Node.firstChild")}}
- {{Domxref("Node.lastChild")}}
- {{Domxref("Node.childNodes")}}
- {{Domxref("Node.nextSibling")}}
- {{Domxref("Node.previousSibling")}}
- {{Domxref("Node.removeChild")}}

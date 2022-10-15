# **[What is TypeScript](https://www.typescripttutorial.net/typescript-tutorial/what-is-typescript/)**

## **What is TypeScript**

TypeScript — это супер набор JavaScript.

TypeScript строится поверх JavaScript. Сначала вы пишете код TypeScript. Затем вы компилируете код TypeScript в простой код JavaScript с помощью компилятора TypeScript.

Получив простой код JavaScript, вы можете развернуть его в любой среде, в которой работает JavaScript.

Файлы TypeScript используют .tsрасширение, а не .jsрасширение файлов JavaScript.

<br/>

![TS to JS](https://www.typescripttutorial.net/wp-content/uploads/2020/05/what-is-typescript-compiler.png)

## **Why TypeScript**

Следующая функция складывает два числа `x` и `y`:

```ts
function add(x, y) {
  return x + y;
}
```

Если вы получите значения из элементов ввода HTML и передадите их в функцию, вы можете получить неожиданный результат

```ts
let result = add(input1.value, input2.value);
console.log(result); // result of concatenating strings
```
Например, если пользователи ввели **10** и **20**, add() функция вернет **1020** вместо **30**.

Причина в том, что ***input1.value*** и ***input2.value*** являются строками, а не числами. Когда вы используете оператор **+** для добавления двух строк, он объединяет их в одну строку.

Когда вы используете TypeScript для явного указания типа параметров, например:

```ts
function add(x: number, y: number) {
   return x + y;
}
```

В этой функции мы добавили числовые типы к параметрам. Функция add() будет принимать только числа, а не какие-либо другие значения.

Когда вы вызываете функцию следующим образом:

```ts
let result = add(input1.value, input2.value);
```

… компилятор TypeScript выдаст ошибку, если вы скомпилируете код TypeScript в JavaScript. Следовательно, вы можете предотвратить возникновение ошибки во время выполнения.


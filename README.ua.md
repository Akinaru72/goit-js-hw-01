# Домашнє завдання №1

## JavaScript. Базові операції та функції

---

## Опис

У цьому домашньому завданні необхідно створити репозиторій **goit-js-hw-01**, підготувати структуру проєкту та реалізувати три базові JavaScript-задачі з використанням функцій, параметрів і шаблонних рядків.

---

## Інструкція

- Створи репозиторій **goit-js-hw-01** та склонюй його собі на комп’ютер.
- У папці `goit-js-hw-01` створи структуру проєкту відповідно до вимог завдання.

![Project preview](assets/homework-js-1.jpg)

- Уважно дотримуйся назв файлів, папок та їх вкладеності — інакше робота не буде прийнята.
- Прочитай кожне завдання та виконай його у відповідному файлі.
- Переконайся, що код відформатований за допомогою **Prettier**.
- Під час відкриття живої сторінки в консолі не повинно бути помилок або попереджень.
- Здай домашнє завдання ментору на платформі **LMS**.

---

## Формат здачі

Домашня робота має містити **два посилання**:

- на вихідні файли (репозиторій з кодом);
- на живу сторінку на **GitHub Pages**.

---

## Задача 1. Замовлення дроїдів

**Файл:** `task-1.js`

Станція з продажу ремонтних дроїдів готова до запуску, залишилося написати програмне забезпечення для відділу продажів.

### Завдання

Оголоси функцію `makeTransaction`, яка приймає два параметри:

- `quantity` — кількість замовлених дроїдів (число);
- `pricePerDroid` — вартість одного дроїда (число).

Функція повинна повертати рядок:

"You ordered <quantity> droids worth <totalPrice> credits!"

де:

- `<quantity>` — кількість замовлених дроїдів;
- `<totalPrice>` — загальна вартість замовлення.

⚠️ Для шаблонних рядків використовуй **тільки бектики (`)**.

### Код для перевірки

```js
console.log(makeTransaction(5, 3000)); // "You ordered 5 droids worth 15000 credits!"
console.log(makeTransaction(3, 1000)); // "You ordered 3 droids worth 3000 credits!"
console.log(makeTransaction(10, 500)); // "You ordered 10 droids worth 5000 credits!"
```

### На що буде звертати увагу ментор при перевірці

- Оголошена функція `makeTransaction(quantity, pricePerDroid)`.
- Виклик `makeTransaction(5, 3000)` повертає `"You ordered 5 droids worth 15000 credits!"`.
- Виклик `makeTransaction(3, 1000)` повертає `"You ordered 3 droids worth 3000 credits!"`.
- Виклик `makeTransaction(10, 500)` повертає `"You ordered 10 droids worth 5000 credits!"`.
- В консоль виведені всі результати викликів.
- Виклик `makeTransaction` з будь-якими валідними аргументами повертає правильне значення.

---

## Задача 2. Доставка товару

**Файл:** `task-2.js`

Оголоси функцію `getShippingMessage`, яка очікує три параметри:

- `country` — країна доставки (рядок);
- `price` — загальна вартість товару (число);
- `deliveryFee` — вартість доставки (число).

Функція повинна повертати рядок:

"Shipping to <country> will cost <totalPrice> credits"

де:

- `<country>` — країна доставки;
- `<totalPrice>` — загальна вартість замовлення, яка включає вартість товару та доставку.

⚠️ Для шаблонних рядків використовуйте **тільки бектики (`)**. Використання одинарних `' '` або подвійних `" "` лапок разом з бектиками є помилкою.

### Код для перевірки

```js
console.log(getShippingMessage("Australia", 120, 50)); // "Shipping to Australia will cost 170 credits"
console.log(getShippingMessage("Germany", 80, 20)); // "Shipping to Germany will cost 100 credits"
console.log(getShippingMessage("Sweden", 100, 20)); // "Shipping to Sweden will cost 120 credits"
```

Залиш цей код для перевірки ментором.

На що буде звертати увагу ментор при перевірці:

- Оголошена функція `getShippingMessage(country, price, deliveryFee)`
- Виклик `getShippingMessage("Australia", 120, 50)` повертає "Shipping to Australia will cost 170 credits"
- Виклик `getShippingMessage("Germany", 80, 20)` повертає "Shipping to Germany will cost 100 credits"
- Виклик `getShippingMessage("Sweden", 100, 20)` повертає "Shipping to Sweden will cost 120 credits"
- Виклик `getShippingMessage` з будь-якими валідними аргументами повертає правильне значення

---

## Задача 3. Ширина елемента

Виконуй це завдання у файлі `task-3.js`.

Оголоси функцію `getElementWidth`, яка очікує три параметри:

- `content` — ширина контенту
- `padding` — значення горизонтального падінгу для кожної зі сторін
- `border` — значення товщини бордера для кожної зі сторін

Значення всіх параметрів будуть рядками формату `Npx`, де `N` — це довільне число, ціле або дробове.

Доповни код функції так, щоб вона повертала число — загальну ширину елемента. При розрахунку загальної ширини орієнтуйся на те, що значення `box-sizing` дорівнює `border-box`.

### Код для перевірки

```js
console.log(getElementWidth("50px", "8px", "4px")); // 74
console.log(getElementWidth("60px", "12px", "8.5px")); // 101
console.log(getElementWidth("200px", "0px", "0px")); // 200
```

Залиш цей код для перевірки ментором.

На що буде звертати увагу ментор при перевірці:

- Оголошена функція `getElementWidth(content, padding, border)`
- Виклик `getElementWidth("50px", "8px", "4px")` повертає число 74
- Виклик `getElementWidth("60px", "12px", "8.5px")` повертає число 101
- Виклик `getElementWidth("200px", "0px", "0px")` повертає число 200
- Виклик `getElementWidth` з будь-якими валідними аргументами повертає правильне значення

---

**Жива сторінка: [GitHub Pages](https://akinaru72.github.io/goit-js-hw-01/)**

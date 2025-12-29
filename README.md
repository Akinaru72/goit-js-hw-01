# Homework #1

## JavaScript. Basic Operations and Functions

---

## Description

In this homework assignment, you need to create a repository **goit-js-hw-01**, prepare the project structure, and implement three basic JavaScript tasks using functions, parameters, and template strings.

---

## Instructions

- Create a repository **goit-js-hw-01** and clone it to your computer.
- In the **goit-js-hw-01** folder, create the project structure according to the task requirements.

![Project preview](assets/homework-js-1.jpg)

- Carefully follow file and folder names and their nesting — otherwise the task will not be accepted.
- Read each task and complete it in the corresponding file.
- Make sure the code is formatted using **Prettier**.
- There should be no errors or warnings in the console when opening the live page.
- Submit the homework to the mentor on the **LMS** platform.

---

## Submission Format

The homework should include **two links**:

- To the source files (repository with code);
- To the live page on **GitHub Pages**.

---

## Task 1. Droid Order

**File:** `task-1.js`

The repair droid sales station is ready to launch, the only thing left is to write the software for the sales department.

### Assignment

Declare a function `makeTransaction` that accepts two parameters:

- `quantity` — the number of droids ordered (number);
- `pricePerDroid` — the price of one droid (number).

The function should return a string:

"You ordered <quantity> droids worth <totalPrice> credits!"

Where:

- `<quantity>` — the number of droids ordered;
- `<totalPrice>` — the total cost of the order.

⚠️ For template strings, use **only backticks (`)**.

### Check Code

```js
console.log(makeTransaction(5, 3000)); // "You ordered 5 droids worth 15000 credits!"
console.log(makeTransaction(3, 1000)); // "You ordered 3 droids worth 3000 credits!"
console.log(makeTransaction(10, 500)); // "You ordered 10 droids worth 5000 credits!"
```

### What the mentor will check

- The function `makeTransaction(quantity, pricePerDroid)` is declared.
- `makeTransaction(5, 3000)` returns `"You ordered 5 droids worth 15000 credits!"`.
- `makeTransaction(3, 1000)` returns `"You ordered 3 droids worth 3000 credits!"`.
- `makeTransaction(10, 500)` returns `"You ordered 10 droids worth 5000 credits!"`.
- All function call results are logged to the console.
- `makeTransaction` with any valid arguments returns the correct value.

## Task 2. Shipping a Product

**File:** `task-2.js`

Declare a function `getShippingMessage` that expects three parameters:

- `country` — the country to ship to (string)
- `price` — the total price of the product (number)
- `deliveryFee` — the shipping fee (number)

The function should return a string:

"Shipping to <country> will cost <totalPrice> credits"

where:

- `<country>` — the destination country;
- `<totalPrice>` — the total order cost, including the item price and delivery.

⚠️ For template strings, use **only backticks (`)**. Using single `' '` or double `" "` quotes together with backticks is incorrect.

### Test Code

```js
console.log(getShippingMessage("Australia", 120, 50)); // "Shipping to Australia will cost 170 credits"
console.log(getShippingMessage("Germany", 80, 20)); // "Shipping to Germany will cost 100 credits"
console.log(getShippingMessage("Sweden", 100, 20)); // "Shipping to Sweden will cost 120 credits"
```

Leave this code for the mentor to check.

What the mentor will pay attention to during the review:

- The function `getShippingMessage(country, price, deliveryFee)` is declared
- Calling `getShippingMessage("Australia", 120, 50)` returns "Shipping to Australia will cost 170 credits"
- Calling `getShippingMessage("Germany", 80, 20)` returns "Shipping to Germany will cost 100 credits"
- Calling `getShippingMessage("Sweden", 100, 20)` returns "Shipping to Sweden will cost 120 credits"
- Calling `getShippingMessage` with any valid arguments returns the correct value

---

## Task 3. Element Width

Complete this task in the file `task-3.js`.

Declare a function `getElementWidth` that expects three parameters:

- `content` — the width of the content
- `padding` — the horizontal padding value for each side
- `border` — the border thickness for each side

All parameter values will be strings in the format `Npx`, where `N` can be any number, integer or fractional.

Complete the function so that it returns a number — the total width of the element. When calculating the total width, assume that `box-sizing` is set to `border-box`.

### Test code

```js
console.log(getElementWidth("50px", "8px", "4px")); // 74
console.log(getElementWidth("60px", "12px", "8.5px")); // 101
console.log(getElementWidth("200px", "0px", "0px")); // 200
```

Leave this code for the mentor to check.

What the mentor will pay attention to during the review:

- The function `getElementWidth(content, padding, border)` is declared
- Calling `getElementWidth("50px", "8px", "4px")` returns the number 74
- Calling `getElementWidth("60px", "12px", "8.5px")` returns the number 101
- Calling `getElementWidth("200px", "0px", "0px")` returns the number 200
- Calling `getElementWidth` with any valid arguments returns the correct value

---

**Live page: [GitHub Pages](https://akinaru72.github.io/goit-js-hw-01/)**

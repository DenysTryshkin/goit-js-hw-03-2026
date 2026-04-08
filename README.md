# Homework: Functions and Conditions

## Task 1: Droid Order with Credits

Declare a function `makeTransaction(quantity, pricePerDroid, customerCredits)` that:

* Calculates total price
* Checks if customer has enough credits

### Returns:

* "Insufficient funds!" if not enough money
* Otherwise:

```
"You ordered <quantity> droids worth <totalPrice> credits!"
```

### Example:

```javascript
console.log(makeTransaction(5, 3000, 23000)); // "You ordered 5 droids worth 15000 credits!"
console.log(makeTransaction(3, 1000, 15000)); // "You ordered 3 droids worth 3000 credits!"
console.log(makeTransaction(10, 5000, 8000)); // "Insufficient funds!"
console.log(makeTransaction(8, 2000, 10000)); // "Insufficient funds!"
console.log(makeTransaction(10, 500, 5000)); // "You ordered 10 droids worth 5000 credits!"
```

---

## Task 2: Message Formatting

Declare a function `formatMessage(message, maxLength)` that:

* Returns original string if length <= maxLength
* Otherwise trims string and adds `...`

### Example:

```javascript
console.log(formatMessage("Curabitur ligula sapien", 16)); // "Curabitur ligula..."
console.log(formatMessage("Curabitur ligula sapien", 23)); // "Curabitur ligula sapien"
console.log(formatMessage("Vestibulum facilisis purus nec", 20)); // "Vestibulum facilisis..."
console.log(formatMessage("Vestibulum facilisis purus nec", 30)); // "Vestibulum facilisis purus nec"
```

---

## Task 3: Spam Check

Declare a function `checkForSpam(message)` that:

* Returns `true` if message contains "spam" or "sale" (case-insensitive)
* Otherwise returns `false`

### Example:

```javascript
console.log(checkForSpam("Latest technology news")); // false
console.log(checkForSpam("Get best sale offers now!")); // true
console.log(checkForSpam("Amazing SalE, only tonight!")); // true
console.log(checkForSpam("Trust me, this is not a spam message")); // true
```

---

## Task 4: Shipping Cost

Declare a function `getShippingCost(country)` using `switch`.

### Shipping prices:

* China — 100 credits
* Chile — 250 credits
* Australia — 170 credits
* Jamaica — 120 credits

### Returns:

```
"Shipping to <country> will cost <price> credits"
```

Or:

```
"Sorry, there is no delivery to your country"
```

### Example:

```javascript
console.log(getShippingCost("Australia")); // "Shipping to Australia will cost 170 credits"
console.log(getShippingCost("Germany")); // "Sorry, there is no delivery to your country"
console.log(getShippingCost("China")); // "Shipping to China will cost 100 credits"
```

---

## Notes

* Use `if...else` for conditions
* Use `switch` where required
* Use `.toLowerCase()` for case-insensitive checks
* Keep test `console.log` for mentor review

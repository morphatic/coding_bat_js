# Sum Double

See: [https://codingbat.com/prob/p141905](https://codingbat.com/prob/p141905)

Given two integer values, return their sum. Unless the two values are the same, then return double their sum.

```js
sumDouble(1, 2) → 3
sumDouble(3, 2) → 5
sumDouble(2, 2) → 8
```

## Project Log

After my first successful iteration, my code looked like this:

```js
const sumDouble = (num1, num2) => {
  if (num1 === num2) {
    return 2 * (num1 + num2)
  } else {
    return num1 + num2
  }
}
```

The final version of my code looks like this:

```js
const sumDouble = (x, y) => (x === y ? 2 : 1) * (x + y)
```

Both of these work. Which one is "better?" The second one is obviously shorter, but arguably it's harder to read. In all likelihood, there is no appreciable difference in how fast they are. In future projects, I'm going to make sure to consider the quality of code, and try to develop and opinion and/or a personal style to how I write things.

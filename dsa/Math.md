### Factorial
```ts
const factorial = (num: number) => {
  if (num === 0 || num === 1) return 1;
  let result = num;
  while (num > 1) {
    num -= 1;
    result *= num;
  }
  return result;
}
```

### Sum from 0 to n
```ts
const sumToN = (n: number) => (n * (n + 1)) / 2;
```
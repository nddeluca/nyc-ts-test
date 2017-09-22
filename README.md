Example showing that `nyc --all ava` does not include `.ts` files that use type casting.

Run `npm test`

`a.js` uses no type casting and is including in the reported coverage.

`b.js` uses `<T>` syntax and is excluded

`c.js uses `as T` syntax and is excluded

If the typecasting is removed, the file will show in the coverage report

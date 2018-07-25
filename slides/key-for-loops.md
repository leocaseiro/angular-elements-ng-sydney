## Key for Loops

<small>
> Uncaught Error: Error trying to diff '[object Object],[object Object]'.
> Only arrays and iterables are allowed
</small>

```
const listItems = numbers.map((number) =>
    <li key={number.toString()}>
      {number}
    </li>
  );
```


https://reactjs.org/docs/lists-and-keys.html

# object spread operator

https://stackoverflow.com/questions/1168807/how-can-i-add-a-key-value-pair-to-a-javascript-object

```js
var obj = {key1: "value1", key2: "value2"};
var pair = {key3: "value3"};
obj = {...obj, ...pair};
console.log(obj);
```

```console
{key1: "value1", key2: "value2", key3: "value3"}
```

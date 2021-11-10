# Decode Message with characters

``` javascript
/* Entries */
const indexes = [5,2,0,1,6,4,8,3,7];
const code = "cdeenetpi";

function decodeMessage(indexes, code) {
  let message = "";
  let index = 0;
  let character = indexes[index];

  while(character != 0) {
    message += code[index];
    index = character;
    character = indexes[index];
  }

  message += code[index];
  return message;
}

/* Show message */
console.log(decodeMessage(indexes,code));

```

``` console
echo "hello world"
```


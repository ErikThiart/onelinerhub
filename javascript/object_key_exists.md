# check if object key exists

```javascript
const object_key_exists = (obj, key) => {
  if(!(typeof obj === 'object' && obj !== null)) return false;
  return Object.keys(obj).includes(key);
}
```

- `object_key_exists` - checks if an object contains the supplied key, returns true if the object contains that key, false otherwise.
- `(obj` - (`Object` type) the object to check its keys.
- `key)` - (`String` type) the key to check its existense in the object.

## Example: 
```javascript
const obj = { a: 1, b:2};
object_key_exists(obj, 'a');
object_key_exists(obj, 'c');
object_key_exists([], 'a');
object_key_exists([], null);
```

true
false
false
false

```

link_youtube: https://youtu.be/U-JyUZo7jAY

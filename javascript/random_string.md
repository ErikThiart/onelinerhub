# Generate random string

```javascript
var chars = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789';
var str = '';
for ( var i = 0; i < 10; i++ ) str += chars.charAt(Math.floor(Math.random() * chars.length));
```

- `var chars` - declare characters string to use for random generation
- `var str` - declare our resulting variable, will contain random string
- `10` - length of random string
- `chars.charAt(Math.floor(Math.random() * chars.length))` - return random character from our ```chars```

group: random_generate


link_youtube: https://youtu.be/UyX_fvabXyw

# Get query parameter value of specified URL

```javascript
(new URL(some_url)).searchParams.get(param);
```

- `new URL` - create native JS URL object to parse specified URL
- `some_url` - URL to parse
- `searchParams` - list of all get parameters
- `(param)` - name of query string parameter to get value of

group: url_components

## Example: 
```javascript
console.log( (new URL('https://example.org/test?id=1')).searchParams.get('id') )
```

"1"
```

group: url_components
```

link_youtube: https://youtu.be/pxboCcS7HBg

# Get cookie with Lua

```nginx
server {
  location / {
    content_by_lua_block {
      local val = ngx.var.cookie_somecookie
      ngx.say(val)
    }
  }
}
```

- `content_by_lua_block` - [lib:nginx-lua](/nginx-lua/how-to-install-nginx-lua-module-in-ubuntu-ubuntuversion) module directive to specify block of Lua code
- `ngx.var.cookie_` - access specified cookie value (comes as a part of variable name)
- `cookie_somecookie` - will return `somecookie` cookie value
- `ngx.say` - output given text to client

group: cookie

## Example: 
```nginx
local val = ngx.var.cookie_somecookie
ngx.say(val)
```
```
123
```

link_youtube: https://youtu.be/1cWkPn-X6Uc

# Add response header with Lua

```nginx
server {
  location / {
    content_by_lua_block {
      ngx.header["X-Example"] = 'onelinerhub-example'
    }
  }
}
```

- `content_by_lua_block` - [lib:nginx-lua](/nginx-lua/how-to-install-nginx-lua-module-in-ubuntu-ubuntuversion) module directive to specify block of Lua code
- `ngx.header` - allows to set response headers
- `X-Example` - sample header to set
- `onelinerhub-example` - sample value to set ([online example](http://lua.onelinerhub.com/set_header))

group: set_header


link_youtube: https://youtu.be/LsCWR8eJBt4

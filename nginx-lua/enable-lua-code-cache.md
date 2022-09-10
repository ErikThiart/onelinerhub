# Enable Lua code cache

```nginx
server {
  location / {
    lua_code_cache on;
    content_by_lua_file /path/to/script.lua;
  }
}
```

- `lua_code_cache` - controls Lua code caching
- `on;` - enables code cache
- `content_by_lua_file` - [lib:nginx-lua](/nginx-lua/how-to-install-nginx-lua-module-in-ubuntu-ubuntuversion) directive to load code from specified Lua code file
- `/path/to/script.lua` - path with Lua code to load

group: code_cahe


link_youtube: https://youtu.be/5xuy_F8b6Q4

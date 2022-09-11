# How to include Lua code from file

### Nginx will cache Lua code from specified file once reloaded. If you want Nginx to load code dynamically, you need to [disable Lua code cache](/nginx-lua/disable-lua-code-cache).

```nginx
server {
  location /test {
    content_by_lua_file /path/to/script.lua;
  }
}
```

- `content_by_lua_file` - [lib:nginx-lua](/nginx-lua/how-to-install-nginx-lua-module-in-ubuntu-ubuntuversion) directive to load code from specified Lua code file
- `/path/to/script.lua` - path with Lua code to load and execute

group: include


link_youtube: https://youtu.be/U_2ZRoU2tPs

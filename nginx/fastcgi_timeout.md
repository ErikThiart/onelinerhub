# Increase FastCGI timeout ("Gateway Timeout" error)

```nginx
server {
  fastcgi_read_timeout 300;
}
```

- `fastcgi_read_timeout 300` - set FastCGI timeout limit to 300 seconds


link_youtube: https://youtu.be/UsuoX9m4wXg

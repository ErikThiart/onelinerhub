# Allow access to single IP address only

```nginx
location / {
  allow 1.2.3.4;
  deny all;
}
```

- `1.2.3.4` - IP address to allow requests from
- `deny all` - will show 403 error (forbidden) for all other IPs

group: block


link_youtube: https://youtu.be/C8S_1YRk9xA

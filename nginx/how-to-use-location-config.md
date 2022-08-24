# How to use location config

```nginx
server {
  # ...
  
  location / {
    root /var/www/website;
  }
}
```

- `server {` - virtual server configuration block
- `location / {` - default location block that will be triggered on all requests
- `root /var/www/website` - set document root for current location block

group: location


link_youtube: https://youtu.be/790d92uGh4Q

# How to use geoip2 module

```nginx
geoip2 /etc/country.mmdb {
  auto_reload 5m;
  $geoip2_data_country_code country iso_code;
}

server {
  if ( $geoip2_data_country_code = "RU" ) {
    return 403 'no no';
  }
}
```

- `geoip2` - [lib:geoip2 module](/nginx/how-to-install-geoip2-modile) directives
- `auto_reload 5m` - check for DB updates every 5 minutes
- `$geoip2_data_country_code` - this variable will store detected country code ([detailed documentation](https://github.com/leev/ngx_http_geoip2_module#description))
- `return 403 'no no';` - forbidden access if country code is `RU`
- `/etc/country.mmdb` - maxmind [geoip database](https://dev.maxmind.com/geoip/geolite2-free-geolocation-data?lang=en) file

group: geoip2


link_youtube: https://youtu.be/X09g6Uz7PUc

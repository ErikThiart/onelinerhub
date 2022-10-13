# Redis pub/sub example

```php
# --- publisher.php ---
ini_set('default_socket_timeout', -1);
$redis->subscribe(['chl'], function($r, $c, $m) {
  # do something with message
});

# --- subscriber.php ---
$redis->publish('chl', 'hi');
```

- `$redis` - Redis object after [connection](/php-redis/how-to-connect-to-redis)
- `subscribe` - subscribe to a specified channel(will wait till message arrived)
- `chl` - channel name to subscribe/publish to
- `function($r, $c, $m)` - callback will be called when new messages arrives
- `publish` - publish message to specified channel
- `'hi'` - message to publish

## Example: 
```php
<?php

$r = new Redis(); 
$r->connect('127.0.0.1', 6379); 

$r->subscribe(['chl'], function($r, $c, $m) {
  die($m);
});

# run this from different script
# $r->publish('chl', 'hi');
```
```
hi
```


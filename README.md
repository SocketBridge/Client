# Client

### Create client
```php
$client = new SocketBridge($token);
```

### Authenticate socket
```php
$client->authenticate(function($channelId, $data) {
  return true;
});
```

### Send data
```php
$client->emit('my-channel', 'start', $data);
```

### Retrieve data
```php
$client->on(function($channelId, $actionName, $data) {
  // Your code
});
```

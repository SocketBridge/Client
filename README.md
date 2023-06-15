# Client

### Create client
```php
$client = new SocketBridge($token);
```

### Send data
```php
$client->emit('my-channel', 'start', $data);
```

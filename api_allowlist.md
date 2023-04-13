## API > Allowlist > IP

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <ipv4>' \
-X GET 'https://api.celltek.space/allowlist/ip'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/allowlist/ip');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <ipv4>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response":{
		"status": <boolean>,
		"ipv4": "<ipv4>",
		"time": <timestamp>
	}
}
```

## API > Allowlist > Domain

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <domain>' \
-X GET 'https://api.celltek.space/allowlist/domain'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/allowlist/domain');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <domain>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response":{
		"status": <httpstatus>,
		"domain": "<domain>",
		"tekbase":{
			"url": "<domain>",
			"dir": "<dir>"
		},
		"money":{
			"money": <number>
		},
		"extensions":{
			<list>
		}
	}
}
```

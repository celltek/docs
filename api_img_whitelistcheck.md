## API > Imageserver Whitelist Check

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <ipv4>' \
-X GET 'https://api.celltek.space/v4/imageserver/whitelist'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/v4/imageserver/whitelist');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <ipv4>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"status": <true|false>,
		"ipv4": "<ipv4>",
		"time": <timestamp>
	}
}
```

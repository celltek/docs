## API > Uptime

> Notice: You need an active API-KEY or you have to wait 300 seconds for the next request 

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/uptime'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/uptime');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"name": "Service Uptime",
		"timestamp": <timestamp>,
		"time": "<date>",
		"space": {
			<list>
		},
		"services": {
			<list>
		}
	}
}
```

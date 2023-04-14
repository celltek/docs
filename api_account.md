## API > Account information

> Notice: You need an active API-KEY
### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/account'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/account');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response":{
		"status": <httpstatus>,
		"tekbase":{
			"url": "<url>",
			"dir": <dir>
		},
		"imageserver":{
			"type": "<type>",
			"access": <boolean>,
			"count": <count>,
			"startdate": <timestamp>,
			"enddate": <timestmap>
		},
		"extensions":{
			<list>
		},
		"dunning":{
			<list>
		}
}
```

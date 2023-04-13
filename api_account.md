## API > Account information

> Notice: You need an active license key

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <license_key>' \
-X GET 'https://api.celltek.space/account'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/account');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <license_key>'
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

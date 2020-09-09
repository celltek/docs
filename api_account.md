## API > Account information

> Notice: You need an active license key

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <license_key>' \
-X GET 'https://api.celltek.space/v4/account'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/v4/account');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <license_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"email": "<email>",
		"url": "<domain>",
		"url_ext": <domain_ext|null>,
		"type": "<Free|Privat|Business>",
		"status": 200,
		"image": {
			"access": <true|false>,
			"count": <count>
			},
		"version": {
			"widget": {
				"tekbase8": "<version>"
			},
			"module": {
				"tekbase8": "<version>"
			},
			"database": {
				"tekbase8": "<version>"
			}
		},
		"shop": {
			<[extensions]>
		},
		"dunning": {
			"status": <false|true>,
			"createtime": <timestamp>,
			"az": "<az>"
		},
		"time": {
			"startdate_at": <timestamp>,
			"enddate_at": <timestamp>,
			"timezone": "UTC/GMT +1"
		},
		"_links": {
			"uri": "https://api.celltek.space/v4/account",
			"time": <timestamp>
		}
	}
}
```

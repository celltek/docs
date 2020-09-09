## API > Addons of a Game by TAG

> Notice: You need an active license key with IP-Whitelist or you have to wait 300 seconds for the next request

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <license_key>' \
-X GET 'https://api.celltek.space/v4/game/addons/<tag>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/v4/addons/<tag>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <license_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"<name>_latest": {
			"name": "<name>",
			"tag": "<tag>",
			"version": {
			"short": <number|latest>,
			"full": <number|latest>
		},
		"files": {
			"file": <url|null>,
			"db_file": "<tag>_latest.zip",
			"db_sha256": null
		},
		"time": {
			"create_at": <timestsamp>,
			"update_at": <timestsamp>,
			"timezone": "UTC/GMT +2"
		},
		"_links": {
			"self": "https://api.celltek.space/v4/game/addon/<tag>/latest",
			"changelog": <url|null>,
			"time": <timestsamp>
		}
},
[..<more>..]
```

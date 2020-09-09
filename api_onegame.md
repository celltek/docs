## API > Specific Game by TAG or GameID

> Notice: You need an active license key with IP-Whitelist or you have to wait 300 seconds for the next request

### Request Example

<!-- tabs:start -->
#### **cURL**

Request with TAG
```cURL
curl -H 'Authorization: <license_key>' \
-X GET 'https://api.celltek.space/v4/game/tag/<tag>'
```

Request with GameID
```cURL
curl -H 'Authorization: <license_key>' \
-X GET 'https://api.celltek.space/v4/game/<gameid>'
```

#### **PHP**


Request with TAG
```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/v4/game/tag/<tag>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <license_key>'
]);
curl_close($ch);
```
Request with GameID
```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/v4/game/<gameid>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <license_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"<linux|windows>": {
		"_id": <number>,
		"name": "<name>",
		"tag": "<tag>",
		"os": "<linux|windows>",
		"ram": <true|false>,
		"mods": <number|false>,
		"addons": <number|false>,
		"appID": <number|false>,
		"steamID": <number|false>,
		"steamLOGIN": <true|false>,
		"steamTOKEN": <true|false>,
		"version": {
		"short": <number>,
		"full": "<number>
		},
	    "image": {
			"icon": "<url>",
			"banner": "<url>",
			"cover_": "<url>"
		},
		"files": {
			"image_file": "<tag>.tar",
			"image_md5": <null|number>,
			"db_file": "<tag_os>.zip",
			"db_sha256": <null|number>
		},
		"status": {
			"percent": <null|number>,
			"text": <null|string>
		},
		"time": {
			"create_at": <timestsamp>,
			"update_at": <timestsamp>,
			"timezone": "UTC/GMT +2"
		},
		"_links": {
			"multi": "https://api.celltek.space/v4/game/tag/<tag>",
			"mods": "https://api.celltek.space/v4/game/mods/<tag> OR <false>",
			"addons": "https://api.celltek.space/v4/game/addons/<tag> OR <false>",
			"changelog": <url|false>,
			"file": <url|false>,
			"time": <timestsamp>
		}
	}
}
```

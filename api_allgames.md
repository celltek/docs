## API > Gamelist

> Notice: You need an active license key with IP-Whitelist or you have to wait 300 seconds for the next request 

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <license_key>' \
-X GET 'https://api.celltek.space/v4/gamelist'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/v4/gamelist');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <license_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
  "<tag>_<os>": {
	"name": "<name>",
	"tag": "<tag>",
	"os": "<linux|windows>",
	"ram": <true|false>,
	"mods": <false|number>,
	"addons": <false|number>,
	"appID": <false|number>,
	"steamID": <false|number>,
	"steamLOGIN": <true|false>,
	"steamTOKEN": <true|false>,
	"version": {
		"short": <number>,
		"full": <number>
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
		"changelog": <url|false>,
		"file": <url|false>,
		"time": <timestsamp>
	}
},
[..<more>..]
```

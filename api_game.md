## API > Game > List

> Notice: You need an active license key with IPv4-Allowlist or you have to wait 300 seconds for the next request 

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <license_key>' \
-X GET 'https://api.celltek.space/game/list'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/game/list');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <license_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
  "{gameTag}": {
	"id": {gameID},
	"name": "{gameName}",
	"tag": "{gameTag}",
	"changelog": "{changelogURL}",
	"link": "https://api.celltek.space/game/{gameTag}",
	"files": {
		"count": {filesCount/null},
		"list": "https://api.celltek.space/game/{gameTag}/files"
	},
	"addons": {
		"count": {addonsCount/null},
		"list": "https://api.celltek.space/game/{gameTag}/addons"
	},
	"mods": {
		"count": {modsCount/null},
		"list": "https://api.celltek.space/game/{gameTag}/mods"
	},
	"version": {
		"short": {versionShort},
		"full": "{versionFull}"
	},
	"steam": {
		"appID": {AppID},
		"steamID": {SteamID},
		"branch": {Branch},
		"mod": {Mod}
	},
	"required": {
		"ram": {true/false},
		"steamLOGIN": {true/false},
		"steamTOKEN": {true/false}
	},
	"image": {
		"icon": "{iconURL}",
		"cover": "{coverURL}",
		"banner": "{bannerURL}",
		"background": "{backgroundURL}",
		"library": "{libraryURL}"
	},
	"file": {
		"tar": "{gameTag}.tar",
		"size": {size},
		"md5": "{md5}",
		"download": "{downloadURL/false}"
	},
	"import": {
		"tekbase": "https://api.celltek.space/game/{gameTag}/import/tekbase"
	},
	"status": {
		"percent": {number},
		"text": "{text/null}"
	},
	"time": {
		"create_at": {timestamp},
		"update_at": {timestamp},
		"timezone": "{timezone}"
	}
  },

[..<more>..]
```

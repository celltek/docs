
> Notice: You need an active API-KEY or you have to wait 300 seconds for the next request 

## API > Game > Tag

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/game/<gameTag>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/game/<gameTag>}');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
  "response": {
	"id": <gameID>,
	"name": "<gameName>",
	"tag": "<gameTag>",
	"changelog": "<changelogURL>",
	"link": "https://api.celltek.space/game/<gameTag>",
	"files": {
		"count": <filesCount>,
		"list": "https://api.celltek.space/game/<gameTag>/files"
	},
	"addons": {
		"count": <addonsCount>,
		"list": "https://api.celltek.space/game/<gameTag>/addons"
	},
	"mods": {
		"count": <modsCount>,
		"list": "https://api.celltek.space/game/<gameTag>/mods"
	},
	"version": {
		"short": <versionShort>,
		"full": "<versionFull>"
	},
	"steam": {
		"appID": <AppID>,
		"steamID": <SteamID>,
		"branch": <Branch>,
		"mod": <Mod>
	},
	"required": {
		"ram": <boolean>,
		"steamLOGIN": <boolean>,
		"steamTOKEN": <boolean>
	},
	"image": {
		"icon": "<iconURL>",
		"cover": "<coverURL>",
		"banner": "<bannerURL>",
		"background": "<backgroundURL>",
		"library": "<libraryURL>"
	},
	"file": {
		"tar": "<gameTag>.tar",
		"size": <size>,
		"md5": "<md5>",
		"download": "<downloadURL>"
	},
	"import": {
		"tekbase": "https://api.celltek.space/game/<gameTag>/import/tekbase"
	},
	"status": {
		"percent": <number>,
		"text": "<text>"
	},
	"time": {
		"create_at": <timestamp>,
		"update_at": <timestamp>,
		"timezone": "<timezone>"
	}
  }
```

## API > Game > Tag > Files

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/game/<gameTag>/files'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/game/<gameTag>}/files');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
"<id>": {
	"name": "<fileName>",
	"path": "<filePath>",
	"addonid": <id>,
	"modid": <id>
},
[..<more>..]
```

## API > Game > Tag > Addons

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/game/<gameTag>/addons'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/game/<gameTag>}/addons');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
"<slug>": {
	"id": <id>,
	"name": "<name>",
	"slug": "<slug>",
	"changelog": "<url>",
	"link": "https://api.celltek.space/game/<gameTag>/addon/<slug>",
	"file": {
		"url": <url>,
		"name": <name>
	},
	"version": {
		"short": "<version>",
		"full": "<version>"
	},
	"time": {
		"create_at": <timestamp>,
		"update_at": <timestamp>
	}
},
[..<more>..]
```

## API > Game > Tag > Mods

> Java Version and Java Path shows only up for Minecraft Modpacks 

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/game/<gameTag>/mods'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/game/<gameTag>}/mods');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
"<slug>": {
	"id": <id>,
	"name": "<name>",
	"slug": "<slug>",
	"changelog": "<url>",
	"link": "https://api.celltek.space/game/<gameTag>/mod/<slug>",
	"file": {
		"url": <url>,
		"name": <name>
	},
	"version": {
		"short": "<version>",
		"full": "<version>"
	},
	"java": {
		"version": "<version>",
		"path": "<path>"
	},
	"time": {
		"create_at": <timestamp>,
		"update_at": <timestamp>
	}
},
[..<more>..]
```

## API > Game > List

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/game/list'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/game/list');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
  "<gameTag>": {
	"id": <gameID>,
	"name": "<gameName>",
	"tag": "<gameTag>",
	"changelog": "<changelogURL>",
	"link": "https://api.celltek.space/game/<gameTag>",
	"files": {
		"count": <filesCount>,
		"list": "https://api.celltek.space/game/<gameTag>/files"
	},
	"addons": {
		"count": <addonsCount>,
		"list": "https://api.celltek.space/game/<gameTag>/addons"
	},
	"mods": {
		"count": <modsCount>,
		"list": "https://api.celltek.space/game/<gameTag>/mods"
	},
	"version": {
		"short": <version>,
		"full": "<version>"
	},
	"steam": {
		"appID": <AppID>,
		"steamID": <SteamID>,
		"branch": <Branch>,
		"mod": <Mod>
	},
	"required": {
		"ram": <boolean>,
		"steamLOGIN": <boolean>,
		"steamTOKEN": <boolean>
	},
	"image": {
		"icon": "<iconURL>",
		"cover": "<coverURL>",
		"banner": "<bannerURL>",
		"background": "<backgroundURL>",
		"library": "<libraryURL>"
	},
	"file": {
		"tar": "<gameTag>.tar",
		"size": <size>,
		"md5": "<md5>",
		"download": "<downloadURL>"
	},
	"import": {
		"tekbase": "https://api.celltek.space/game/<gameTag>/import/tekbase"
	},
	"status": {
		"percent": <number>,
		"text": "<text>"
	},
	"time": {
		"create_at": <timestamp>,
		"update_at": <timestamp>,
		"timezone": "<timezone>"
	}
  },

[..<more>..]
```

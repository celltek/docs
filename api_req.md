
> Notice: You need an active API-KEY or you have to wait 300 seconds for the next request 

## API > Requests > IP

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/req/ip/<ipv4|ipv6>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/req/ip/<ipv4|ipv6>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"short": {
			<short_list>
		},
		"<details>"{
			<details_list>
		},
	}
}
```

## API > Requests > SSL Scan

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/req/sslscan/<domain>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/req/sslscan/<domain>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"host": "<domain>",
		"port": <port>,
		"protocol": "<protocol>",
		"isPublic": <boolean>,
		"status": "<text>",
		"startTime": <timestamp>,
		"engineVersion": "<version>",
		"criteriaVersion": "<version>",
		"<endpoints>"{
			<endpoints_list>
		},
	}
}
```

## API > Requests > Steam > SteamID

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/req/steam/<steamID>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/req/steam/<steamID>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"name": "<name>",
		"buildid": <version>,
		"branch": "<branch>"
	}
}
```

## API > Requests > Steam > SteamID & Branch

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/req/steam/<steamID>/<steamBranch>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/req/steam/<steamID>/<steamBranch>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"name": "<name>",
		"buildid": <version>,
		"branch": "<branch>"
	}
}
```

## API > Requests > Minecraft > Plugin

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/req/minecraft/plugin/<id>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/req/minecraft/plugin/<id>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"file": "<url>",
		"name": "<name>",
		"gameVersion": <version>,
		"url": "<url>",
		"buildid": <version>
	}
}
```
## API > Requests > Minecraft > Modpack

> Notice: Store TP does not need an ID but the SLUG 

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/req/minecraft/modpack/<cf|ftb|tp>/<id>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/req/minecraft/modpack/<cf|ftb|tp>/<id>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"name": "<name>",
		"author": "<name>",
		"description": "<description>",
		"image": "<url>",
		"url": "<url>",
		"file": "<url>",
		"dateReleased": <timestamp>,
		"dateCreated": <timestamp>,
		"dateModified": <timestamp>,
		"buildid": "<version>"
	}
}
```
## API > Requests > TruckerMP > Version

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/req/tmp/version'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/req/tmp/version');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"name": "<string>",
		"numeric": <int>,
		"stage": "<string>",
		"ets2mp_checksum": {
		"dll": "<string>",
		"adb": "<string>"
		},
		"atsmp_checksum": {
		"dll": "<string>",
		"adb": "<string>"
		},
		"time": "<string>",
		"supported_game_version": "<string>",
		"supported_ats_game_version": "<string>"
	}
}
```

## API > Requests > TruckerMP > Time

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/req/tmp/time'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/req/tmp/time');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"timestamp": <int>,
		"time": "<string>"
	}
}
```

## API > Requests > TruckerMP > Server

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/req/tmp/server'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/req/tmp/server');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": [
		{
		"id": <int>,
		"game": "<string>",
		"ip": "<string>",
		"port": <int>,
		"name": "<string>",
		"shortname": "<string>",
		"idprefix": "<string>",
		"online": <boolean>,
		"players": <int>,
		"queue": <int>,
		"maxplayers": <int>,
		"mapid": <int>,
		"displayorder": <int>,
		"speedlimiter": <int>,
		"collisions": <boolean>,
		"carsforplayers": <boolean>,
		"policecarsforplayers": <boolean>,
		"afkenabled": <boolean>,
		"event": <boolean>,
		"specialEvent": <boolean>,
		"promods": <boolean>,
		"syncdelay": <int>
		},
		[LIST]
	]
}
```

## API > Requests > TruckerMP > Server > ID

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/req/tmp/server/<id>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/req/tmp/server/<id>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response":
		{
		"id": <int>,
		"game": "<string>",
		"ip": "<string>",
		"port": <int>,
		"name": "<string>",
		"shortname": "<string>",
		"idprefix": "<string>",
		"online": <boolean>,
		"players": <int>,
		"queue": <int>,
		"maxplayers": <int>,
		"mapid": <int>,
		"displayorder": <int>,
		"speedlimiter": <int>,
		"collisions": <boolean>,
		"carsforplayers": <boolean>,
		"policecarsforplayers": <boolean>,
		"afkenabled": <boolean>,
		"event": <boolean>,
		"specialEvent": <boolean>,
		"promods": <boolean>,
		"syncdelay": <int>
		}
}
```

## API > Requests > TruckerMP > Server MapID > ID

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/req/tmp/server/mapid/<id>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/req/tmp/server/mapid/<id>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response":
		{
		"id": <int>,
		"game": "<string>",
		"ip": "<string>",
		"port": <int>,
		"name": "<string>",
		"shortname": "<string>",
		"idprefix": "<string>",
		"online": <boolean>,
		"players": <int>,
		"queue": <int>,
		"maxplayers": <int>,
		"mapid": <int>,
		"displayorder": <int>,
		"speedlimiter": <int>,
		"collisions": <boolean>,
		"carsforplayers": <boolean>,
		"policecarsforplayers": <boolean>,
		"afkenabled": <boolean>,
		"event": <boolean>,
		"specialEvent": <boolean>,
		"promods": <boolean>,
		"syncdelay": <int>
		}
}
```

## API > Requests > TruckerMP > Player > TruckerID|SteamID64

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/req/tmp/player/<truckerid|steamid64>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/req/tmp/player/<truckerid|steamid64>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"id": <int>,
		"name": "<string>",
		"avatar": "<string>",
		"smallAvatar": "<string>",
		"joinDate": "<string>",
		"steamID64": <int>,
		"steamID": <int>,
		"discordSnowflake": null,
		"displayVTCHistory": <boolean>,
		"groupName": "<string>",
		"groupColor": "<string>",
		"groupID": <int>,
		"banned": <boolean>,
		"bannedUntil": null,
		"bansCount": <int>,
		"displayBans": <boolean>,
		"patreon": {
		"isPatron": true,
		"active": <boolean>,
		"color": null,
		"tierId": null,
		"currentPledge": null,
		"lifetimePledge": <int>,
		"nextPledge": null,
		"hidden": <boolean>
		},
		"permissions": {
		"isStaff": <boolean>,
		"isUpperStaff": <boolean>,
		"isGameAdmin": <boolean>,
		"showDetailedOnWebMaps": <boolean>
		},
		"vtc": {
		"id": <int>,
		"name": "<string>",
		"tag": "<string>",
		"inVTC": <boolean>,
		"memberID": <int>
		},
		"vtcHistory": null
		}
}
```

## API > Requests > TruckerMP > Online > Search > Query

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/req/tmp/online/search/<query>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/req/tmp/online/search/<query>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": [
		{
		"id": <int>,
		"name": "<string>",
		"avatar": "<string>",
		"profile": "<string>",
		"joinDate": "<string>",
		"groupName": "<string>",
		"banned": false,
		"bansCount": <int>,
		"bannedUntil": null,
		"gps": {
			"playerId": <int>,
			"X": <int>,
			"Y": <int>,
			"follow": "<string>"
		},
		"server": {
			"game": "<string>",
			"name": "<string>",
			"traffic": [
				"<string>",
				"<string>",
				"<string>",
				"<string>",
				"<string>",
				"<string>",
				"<string>",
				"<string>",
				"<string>",
				"<string>"
			],
			"url": "<string>"
		}
		},
		[LIST]
	]
}
```


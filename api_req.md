
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

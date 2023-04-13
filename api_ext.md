
> Notice: You need an active license key or you have to wait 300 seconds for the next request 

## API > Extensions > ID

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <license_key>' \
-X GET 'https://api.celltek.space/ext/<id>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/ext/<id>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <license_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"id": <id>,
		"name": "<name>",
		"link": "https://www.celltek.space/extensions/<id>",
		"changelog": "<url>",
		"version": {
			"full": "<version>",
			"short": <version>
		},
		"required": {
			"tekbase": "<version>",
		"dependices": [
			<list>
			]
		},
		"vendor": {
			"publisher": "<name>",
			"verified": <boolean>,
			"url": "<url>",
			"privacypolice": "<url>",
			"support": "<url>"
		},
		"shop": {
			"category": "<name>",
			"catid": <id>,
			"price": <price>,
			"currency": "<currency>",
			"fees": "<pirce>",
			"term": "<number>"
		},
		"time": {
			"create_at": <timestamp>,
			"update_at": <timestamp>
		}
	}
}
```

## API > Extensions > Cats

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <license_key>' \
-X GET 'https://api.celltek.space/ext/cats'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/ext/cats');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <license_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"list": [
			{
			"id": <id>,
			"title": "<name>",
			"icon": "<string>",
			"count": <number>
			},
			<more>
		]
	}
}
```

## API > Extensions > List

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <license_key>' \
-X GET 'https://api.celltek.space/ext/list'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/ext/list');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <license_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"list": [
		{
			"id": <id>,
			"name": "<name>",
			"link": "https://www.celltek.space/extensions/<id>",
			"changelog": "<url>",
			"version": {
				"full": "<version>",
				"short": <version>
			},
			"required": {
				"tekbase": "<version>",
			"dependices": [
				<list>
				]
			},
			"vendor": {
				"publisher": "<name>",
				"verified": <boolean>,
				"url": "<url>",
				"privacypolice": "<url>",
				"support": "<url>"
			},
			"shop": {
				"category": "<name>",
				"catid": <id>,
				"price": <price>,
				"currency": "<currency>",
				"fees": "<pirce>",
				"term": "<number>"
			},
			"time": {
				"create_at": <timestamp>,
				"update_at": <timestamp>
			}
		},
		<more>
		]
	}
}
```

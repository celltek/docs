
> Notice: You need an active API-KEY or you have to wait 300 seconds for the next request 

## API > Denylist > Domains

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/denylist/domains'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/denylist/domain');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response":{
		"list": [
			{
				"id": <id>,
				"name": "<url>"
			},
			<more>
		]
	}
}
```

## API > Denylist > Phones

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/denylist/phones'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/denylist/phones');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response":{
		"list": [
			{
				"name": "<number>"
			},
			<more>
		]
	}
}
```

## API > Denylist > Words

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/denylist/words'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/denylist/words');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response":{
		"list": [
			{
				"name": "<string>"
			},
			<more>
		]
	}
}
```
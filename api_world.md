
> Notice: You need an active API-KEY or you have to wait 300 seconds for the next request 

## API > World

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <api_key>' \
-X GET 'https://api.celltek.space/world/<iso2|iso3>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/world/<iso2|iso3>');
curl_setopt($ch, CURLOPT_HTTPHEADER, [
  'Authorization: <api_key>'
]);
curl_close($ch);
```
<!-- tabs:end -->

```json
{
	"response": {
		"country": {
			"name": "<string>",
			"native": "<string>",
			"capital": "<string>",
			"region": "<string>",
			"subregion": "<string>",
			"tld": "<string>",
			"phone_code": <number>,
			"country_code": {
			"iso3": "<string>",
			"iso2": "<string>"
			},
			"timezones": [
			{
			"zoneName": "<string>",
			"gmtOffset": <number>,
			"gmtOffsetName": "<string>",
			"abbreviation": "<string>",
			"tzName": "<string>"
			},
			{
			"zoneName": "<string>",
			"gmtOffset": <number>,
			"gmtOffsetName": "<string>",
			"abbreviation": "<string>",
			"tzName": "<string>"
			}
			],
			"translations": {
			"br": "<string>",
			"pt": "<string>",
			"nl": "<string>",
			"hr": "<string>",
			"fa": "<string>",
			"de": "<string>",
			"es": "<string>",
			"fr": "<string>",
			"ja": "<string>",
			"it": "<string>"
			},
			"latitude": <number>,
			"longitude": <number>
			}
	}
}
```

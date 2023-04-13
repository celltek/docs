
> Notice: You need an active license key or you have to wait 300 seconds for the next request 

## API > Github > Repo

### Request Example

<!-- tabs:start -->
#### **cURL**

```cURL
curl -H 'Authorization: <license_key>' \
-X GET 'https://api.celltek.space/git/repo/<name>'
```

#### **PHP**

```php
$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, 'https://api.celltek.space/git/repo/<name>');
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
		"url": "<url>",
		"file": "<url>",
		"version": "<verson>",
		"time": {
			"created_at": "<timestamp>",
			"updated_at": "<timestamp>"
		}
	}
}
```

## API > RESTful-API System

> Notice: No cURL request only Browser

### Request Example

```web
// URL
https://api.celltek.space/v4/system
```

```json
{
	"response": {
		"name": "RESTful-API",
		"author": "celltek.space",
		"version": "<number>",
		"system": {
			"php": "<number>",
			"mysql": "<string>",
			"timestamp": <timestamp>,
			"time": "<date>",
			"timezone": "UTC/GMT +2"
		},
		"tekbase": {
		"changelog": "<number>",
		"database": "<number>",
		"module": "<number>",
		"widget": "<number>"
		},
		"module": {
		"openssl": <true|false>,
		"curl": <true|false>,
		"geoip": <true|false>,
		"mysqli": <true|false>,
		"ssh2": <true|false>,
		"ionCube Loader": "<number>,"
		},
		"_links": {
		"self": "https://api.celltek.space/v4/system"
		}
	}
}
```

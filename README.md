# shorten-with-lanza.me
Shorten URL using Lanza.me shortener

Install with npm i shorten-with-lanza.me

```javascript
	var lanzame = require('shorten-with-lanza.me')

	lanzame.shorten({_id: '1234567890', url: 'google.es'}).then(function(json){
		
		if(json.shortUrl){
			console.log('OK ', json.shortUrl) // ok
		}else{
			console.log('FAIL ', json.error) // fail some option, probably
		}
		
	}).catch(function(err){
		
		console.log('ERROR ', err.error)	// a error message
		console.log('FALLB ', err.shortUrl) // fallback, returns the original long url
		
	})
```


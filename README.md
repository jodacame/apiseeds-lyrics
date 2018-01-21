# Apiseeds | Lyrics

Is a simple module that provides lyrics from https://apiseeds.com/ directly into your js file in JSON format.

## Requeriments
* FREE Api key from https://apiseeds.com/

## Method

**getLyric**

### Params 

* apikey (String) [Required]
* artist (String) [Required]
* track (String) [Required]
* callback(response,headers) (Function) [Required]

## Installation
```Bash
# Local installation
npm install -s apiseeds-lyrics

# Global installation
npm install -g apiseeds-lyrics

```
## Example

```Javascript
'use strict';

var lyrics = require("apiseeds-lyrics");

const apikey = 'YOUR-API-KEY';

lyrics.getLyric(apikey,"The Beatles","Yesterday",function(response,headers){
    console.log("Header", headers);
    console.log("Response",response);
});
```

## Important 

Rate limit and credits are in the header response

## Api Documentation 

https://apiseeds.com/documentation/lyrics
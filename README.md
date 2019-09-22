
## Description
Module non-officiel pour l'api du bot Améthyse

## Installation

## Endpoint

 - url = Image url
 - pixelize (entre 1 et 50, default: 8)
 - posterize (entre 1 et 100, defaut : 5 )
 - blur (entre 1 et 30, defaut : 5)


|Nom|Params|
|--|--|
|circle|url|
|rejected|url|
|approved|url|
|glitch|url|
|distort|url|
|sepia|url|
|contrast|url|
|greyscale|url|
|invert|url|
|pixelize|url, pixelize|
|blur|url, blur|
|posterize|url, posterize|
|beautiful|url|
|wanted|url|
|3000years|url|


## Utilisation
```
npm i amethyse-api
```

**Connexion :**
```js
    const ameClient = require(******)
    const ameApi = new ameClient(client, "token")
```
**Endpoint :**
```js
    let image = ameApi.generate("endpoint", {
	    "url" : "image url"
    })
    console.log(image)
```
*Returns*
```
<Buffer ... >
```
**Endpoint  Exemple:**
```js
    let image = ameApi.generate("glitch", {
	    "url" : "https://cdn.discordapp.com/avatars/450352584302002186/c0ff7e943ab89560503b8e99591ff888.png?size=2048"
    })
    console.log(image)
```
*Returns*
```
<Buffer ... >
```
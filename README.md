R - CHNWT
=========

R - CHNWT is a URL shortener to reduce a long link.

API
---
This API is based on HTTPS / JSON requests and responses. `https://r.chnwt.dev`

### Create a shortened URL

##### API request
`POST /url`
<details>
<summary>JSON</summary>

```json
{
    "url": "[:fullURL]"
}
```
</details>

##### API response
<details>
<summary>JSON</summary>

```json
{
    "status": "success",
    "id": "[:id]",
    "shortUrl": "https://r.chnwt.dev/[:id]",
    "fullUrl": "[:fullURL]"
}
```
</details>


### Shortened URL redirect

##### HTTPS request
`GET /[:id]`

##### HTTPS response
`Redirect to full URL`

_____

## Requirements

- Node LTS

## Installation

```sh
$ npm install
$ npm run start
```

or

```sh
$ yarn
$ yarn start
```

## Config

create .env file

```
FIREBASE='{"apiKey": "","authDomain": "","databaseURL": "","projectId": "","storageBucket": "","messagingSenderId": "","appId": ""}'
```

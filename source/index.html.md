---
title: "Auslan Connections App API"
language_tabs:
  - json: JSON
  - shell: cURL
---

# Users

## Getting a list of users


### Request

#### Endpoint

```
GET /api/v1/users
Accept: application/json
Content-Type: application/json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOjV9.jxJFCXmk8SOCtmmHqczBlZZEra1qa8xly7zWZ42EnO4
Host: example.org
Cookie: 
```

`GET /api/v1/users`

#### Parameters


None known.


### Response

```
X-Frame-Options: SAMEORIGIN
X-XSS-Protection: 1; mode=block
X-Content-Type-Options: nosniff
Content-Type: application/json; charset=utf-8
ETag: W/&quot;2bcea2f068831928fa6159a99dd963dc&quot;
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: 579e0844-cb34-488a-b834-dad805e62f28
X-Runtime: 0.054005
Vary: Origin
Content-Length: 171
200 OK
```


```json
{
  "users": [
    {
      "id": 5,
      "type": "Administrator",
      "email": "robin@auslan.com.au",
      "first_name": "Robin",
      "last_name": "Boss",
      "mobile": "0400 000 000",
      "verified": false,
      "disabled": false
    }
  ]
}
```



```shell
curl "https://auslan.herokuapp.com/api/v1/users" -X GET \
	-H "Accept: application/json" \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOjV9.jxJFCXmk8SOCtmmHqczBlZZEra1qa8xly7zWZ42EnO4" \
	-H "Host: example.org" \
	-H "Cookie: "
```

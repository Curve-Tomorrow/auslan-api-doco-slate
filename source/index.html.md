---
title: "Auslan Connections App API"
language_tabs:
  - json: JSON
  - shell: cURL
---

# Users

## Getting a list of users

This method gets all users.

### Request

#### Endpoint

```
GET /api/v1/users
Accept: application/json
Content-Type: application/json
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOjMzfQ.8_qqCkuH1ZAd_GsMOyakdV1LQC6faoRWNZfFQiCYK-c
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
ETag: W/&quot;b017d80844ce34659b256923f1afc9ea&quot;
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: 2c8ad9fc-bb7d-445f-a99c-0c7964ece52c
X-Runtime: 0.038804
Vary: Origin
Content-Length: 513
200 OK
```


```json
{
  "users": [
    {
      "id": 35,
      "type": "Accountant",
      "email": "melissa@auslan.com.au",
      "first_name": "Melissa",
      "last_name": "Spy",
      "mobile": "0400 000 000",
      "verified": false,
      "disabled": false
    },
    {
      "id": 34,
      "type": "OrganisationalRepresentative",
      "email": "alana@auslan.com.au",
      "first_name": "Alana",
      "last_name": "Matthews",
      "mobile": "0400 000 000",
      "verified": false,
      "disabled": false
    },
    {
      "id": 33,
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
	-H "Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOjMzfQ.8_qqCkuH1ZAd_GsMOyakdV1LQC6faoRWNZfFQiCYK-c" \
	-H "Host: example.org" \
	-H "Cookie: "
```

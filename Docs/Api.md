# Buber Dinner API

- [Buber Dinner API](#buber-dinner-api)
  - [Auth](#auth)
    - [Register](#register)
      - [Register Request](#register-request)
      - [Register Response](#register-response)
    - [Login](#login)
      - [Login Request](#login-request)
      - [Login Response](#login-response)

## Auth

### Register

```js
POST {{host}}/auth/register
```

#### Register Request

```json
{
  "firstName": "Nurs",
  "lastName": "Still",
  "email": "nurs@still.com",
  "password": "Nst123!"
}
```

#### Register Response

```js
200 OK
```

```json
{
  "id": "d89c2d9a-eb2a-4067-95ff-b529b55za195",
  "firstName": "Nurs",
  "lastName": "Still",
  "email": "nurs@still.com",
  "token": "eyJhb...z9djcnXoy"
}
```

### Login

```js
POST {{host}}/auth/login
```

#### Login Request

```json
{
  "email": "nurs@still.com",
  "password": "Nst123!"
}
```

#### Login Response

```js
200 OK
```

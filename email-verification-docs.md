# Zuri Chat Core Email Verification API (1.0.0)

## End-Point

<details>
  <summary> POST /auth/verify/mail </summary>
Zuri Chat Core Email Verification API

https://api.zuri.chat/auth/verify/mail

 </details>

## Authentication request to access protected resources

```
REQUEST BODY SCHEMA: application/json

code               String

```

## Sample request

How to make an email verification request

**content type** <br> application/json

```
{
    "code": "893723"
}
```

## Responses

### **200** verification successful <br>

```
RESPONSE SCHEMA: application/json

status required      integer <int32>
message required   string
data required      object

```

## Response Sample

**Content type** <br>
application/json

```
{
"status": 200,
"message": "string",
- "data": {
<!-- unknown for now -->
}
}
```

Response for 4xx and 5xx requires the int error code and a string message. For example; <br>

**Content type** <br>
application/json

```
{

"status": 400,
"message": "string"

}

```

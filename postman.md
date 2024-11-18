Для репрезентации опыта работы с Posеnman буду использовать изменение профиля в интернет магазине https://alikson.ru/

**Bearer token:** eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNzMxOTQ2NDk5LCJpYXQiOjE3MzE5NDMxOTksImp0aSI6ImRlYzI2ZmQyMDNhYjQ5YjJiYWE3NmUxNzM5MjVjYzgyIiwidXNlcl9pZCI6MzcyNTF9.6FDxTEkuIawk-BN-zWCauBD01Xk2X3lOPTCQEM1wpkI

**PUT:** https://alikson.ru/api/lk/personal/update/

**Body (Payload):**
```JSON
{
  "email": "asd@пgmail.com",
  "username": "asd@пgmail.com",
  "first_name": "Aski",
  "last_name": "Qasil",
  "phone": "+7-923-415-78-12"
}
```
**Response:**<br>
**Status:** 200 Ok
```JSON
{
  "email": "asd@пgmail.com",
  "username": "asd@пgmail.com",
  "first_name": "Aski",
  "last_name": "Qasil",
  "phone": "+7-923-415-78-12"
  "is_active": true
}
```

API Testing

Авторизация пользователя

Request

POST /api/login

{
  "email": "user@test.ru",
  "password": "Password123!"
}

Expected Response

Status Code: 200 OK

{
  "token": "jwt_token",
  "userId": 15
}

⸻

Неверный пароль

Request

POST /api/login

{
  "email": "user@test.ru",
  "password": "WrongPassword"
}

Expected Response

Status Code: 401 Unauthorized

{
  "message": "Неверные учетные данные"
}
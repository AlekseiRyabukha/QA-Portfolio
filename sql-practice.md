SQL Practice for QA

Проверка существования пользователя

SELECT *
FROM users
WHERE email = 'user@test.ru';

⸻

Проверка количества активных пользователей

SELECT COUNT(*)
FROM users
WHERE is_active = 1;

⸻

Проверка последнего входа пользователя

SELECT email, last_login
FROM users
WHERE email = 'user@test.ru';

⸻

Проверка заказов пользователя

SELECT *
FROM orders
WHERE user_id = 15;

⸻

Проверка количества заказов по статусам

SELECT status, COUNT(*)
FROM orders
GROUP BY status;

⸻

Поиск дублирующихся email

SELECT email, COUNT(*)
FROM users
GROUP BY email
HAVING COUNT(*) > 1;

⸻

Проверка пользователей без заказов

SELECT u.id, u.email
FROM users u
LEFT JOIN orders o ON u.id = o.user_id
WHERE o.id IS NULL;

⸻

Проверка последних зарегистрированных пользователей

SELECT *
FROM users
ORDER BY created_at DESC
LIMIT 10;
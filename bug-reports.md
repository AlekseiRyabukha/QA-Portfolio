Bug Reports

⸻

BUG-001

Summary

После выхода из системы пользователь может получить доступ к личному кабинету через кнопку “Назад” в браузере.

Environment

* Windows 11
* Google Chrome 136.0
* Production

Preconditions

Пользователь авторизован в системе.

Steps to Reproduce

1. Выполнить вход в систему.
2. Перейти в личный кабинет.
3. Нажать кнопку “Выйти”.
4. Нажать кнопку “Назад” в браузере.

Expected Result

Пользователь перенаправляется на страницу авторизации.

Actual Result

Отображается содержимое личного кабинета.

Severity

High

Priority

High

⸻

BUG-002

Summary

Система принимает email без символа “@” при восстановлении пароля.

Environment

* Windows 11
* Google Chrome 136.0
* Production

Preconditions

Открыта страница восстановления пароля.

Steps to Reproduce

1. Перейти на страницу восстановления пароля.
2. Ввести значение “testmail.ru”.
3. Нажать кнопку отправки.

Expected Result

Отображается сообщение о неверном формате email.

Actual Result

Форма успешно отправляется.

Severity

Medium

Priority

High

⸻

BUG-003

Summary

Кнопка “Войти” становится активной при незаполненных обязательных полях.

Environment

* Windows 11
* Google Chrome 136.0
* Production

Preconditions

Открыта страница авторизации.

Steps to Reproduce

1. Оставить поля логина и пароля пустыми.
2. Проверить состояние кнопки “Войти”.

Expected Result

Кнопка недоступна до заполнения обязательных полей.

Actual Result

Кнопка активна.

Severity

Medium

Priority

Medium

⸻

BUG-004

Summary

После пяти неудачных попыток входа учетная запись не блокируется.

Environment

* Windows 11
* Google Chrome 136.0
* Production

Preconditions

Существует активная учетная запись.

Steps to Reproduce

1. Ввести корректный логин.
2. Пять раз подряд вводить неверный пароль.
3. Повторить попытку входа.

Expected Result

Учетная запись временно блокируется либо появляется ограничение на повторные попытки.

Actual Result

Количество попыток не ограничено.

Severity

Critical

Priority

Critical

⸻

BUG-005

Summary

После смены пароля старый пароль продолжает работать.

Environment

* Windows 11
* Google Chrome 136.0
* Production

Preconditions

Пользователь зарегистрирован в системе.

Steps to Reproduce

1. Выполнить смену пароля.
2. Выйти из системы.
3. Выполнить вход со старым паролем.

Expected Result

Старый пароль недействителен.

Actual Result

Авторизация выполняется успешно.

Severity

Critical

Priority

Critical
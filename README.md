# Лабораторная работа 1

## Задание
- Спроектировать и разработать систему авторизации пользователей на протоколе HTTP.

## Ход работы
- Разработка пользовательского интерфейса и описание сценариев работы

Изначально пользователь попадает на главную страницу авторизации - `index.php`, на которой будет предложено сразу войти в аккаунт или зарегистрироваться с нуля. Пользователь увидит поля `Логин`и `Пароль`, а так же кнопку `Войти` и  надпись `зарегистрируйтесь`. Если пользователь уже регистрировался, то при корректном вводе логина и пароля его переадресует на страничку профиля - `profile.php`. В случае некорректного ввода данных пользователь увидит окно `Неверный логин или пароль` под формой авторизации. 

- Схема процесса авторизации

![autorization scheme](/schemes/1.png "autorization scheme")

Если пользователю необходимо зарегистрироваться, он переходит на страничку `register.php` путём нажатия на гиперссылку в слове `зарегистрируйтесь`. Пользователя встречает форма регистрации, содержащая некоторые поля для данных и предлагается загрузить собственную картинку профиля. По мере заполнения формы, пользователь должен убедиться, что поля `Пароль` и `Подтверждение пароля` содержат одинаковое значение. В случае, если данные поля отличаются содержимым и пользователь нажимает `Войти`, под окном регистрации появится уведомление `Пароли не совпадают` и прийдётся заполнять все строки заново. В ином же случае, пользователя переадресует на страничку входа, и под формой авторизации будет уведомление `Регистрация прошла успешно`.

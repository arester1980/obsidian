Check-list
## 1. Функциональное тестирование

### Тестирование форм

1. Регистрация

- Пользователь с данными существует в системе.
- Пользователь с данными не существует в системе.
- Пользователь, заблокированный в системе, не может пройти повторную регистрацию.

2. Авторизация

- Пользователь существует в системе с введенным логином и паролем.
- Пользователь с введенным логином не существует в системе.
- Пользователь с введенным логином существует в системе, но пароль неверный.
- Пользователь с введенным логином и паролем существует в системе, но заблокирован модерацией (страница заморожена).
- Валидация полей ввода.

3. Протестируйте валидацию всех обязательных полей

- Максимальная и минимальная длина.
- Диапазон допустимых символов, спецсимволы.
- Обязательность к заполнению.
- Убедитесь, что астериск (знак звездочки) отображается у всех обязательных полей.
- Убедитесь, что система не отображает окно ошибки при незаполненных необязательных полях.

4. Формы обратной связи
5. Ссылки на пользовательские соглашения

### Поиск

1. Результаты существуют/не существуют.
2. Корректное сообщение о пустом результате.
3. Пустой поисковой запрос.
4. Поиск по эмодзи.

### Поля

1. Числовые поля: они не должны принимать буквы, в этом случае должно отображаться соответствующее сообщение об ошибке.
2. Дробные значения, например, как система валидирует 1.1 и 1,1.
3. Отрицательные значения в числовых полях, если они разрешены.
4. Деление на ноль корректно обрабатывается.
5. Протестируйте максимальную длину каждого поля, чтобы убедиться, что данные не обрезаются или скрываются под многоточие.
6. Протестируйте все поля ввода на спецсимволы.
7. Проверить что текст не выезжает за границы поля.

### Всплывающие сообщения

1. Протестируйте всплывающие сообщения («Это поле ограничено N знаками»).
2. Подтверждающие сообщения отображается для операций обновления и удаления.
3. Сообщения об ошибках ввода.

### Фильтры

1. Протестируйте функциональность сортировки (по возрастанию, по убыванию, по новизне).
2. Задать фильтры с выдачей.
3. Задать фильтры, по которым нет выдачи.
4. Фильтры по категориям/подкатегориям.
5. Фильтры с радиусом поиска.
6. Данные в выпадающих списках.

### Other

1. Протестируйте функциональность доступных кнопок.
2. Наличие favicon.
3. Проверка обработки различных ошибок (страница не найдена, тайм-аут, ошибка сервера и т.д.).
4. Протестируйте, что все загруженные документы правильно открываются.
5. Пользователь может скачать/прикрепить/загрузить файлы/медиа (картинки, видео и т.д.). А также удалить эти файлы из вложений. Убедитесь, что файлы уходят на сервер только после нажатия соответствующей кнопки
6. Протестируйте почтовую функциональность системы.

### Кеш, cookie и сессии

1. Пользователь очистил кэш браузера
2. Посмотрите, что будет, если пользователь удалит куки, находясь на сайте.
3. Посмотрите, что будет, если пользователь удалит куки после посещения сайта.

### DevTools

1. Ошибки в Console.
2. Все стили загружаются.
3. Картинки загружаются.

---

## 2. Интеграционное тестирование

- Проверяем работу сторонних модулей: оплата, шаринг, карты.
- Реклама (просмотр, переходы по рекламе, аналитика).
- Метрики (переходы по страницам, показы элементов, клики).

---

## 3. Тестирование безопасности

1. Пользователь не может авторизоваться: под старым паролем, заблочен в сервисе, достиг лимита авторизаций, ввел чужой код верификации.
2. Страницы, содержащие важные данные (пароль, номер кредитной карты и CVC, ответы на секретные вопросы и т. п.) открываются через HTTPS (SSL).
3. Пароль скрыт астерисками на страницах: регистрация, «забыли пароль», «смена пароля».
4. Корректное отображение сообщений об ошибках.
5. Завершение сесcии после разлогина.
6. Доступ к закрытым разделам сайта.
7. SQL-инъекции.
8. Cross-Site Scripting (XSS) уязвимости.
9. HTML-инъекции.
10. Cookie должны храниться в зашифрованном виде.
11. Роли пользователей и доступ к контенту.

---

## 4. Тестирование локализации и глобализации

1. Дата и время. Например отображение времени, даты в соответствии с часовым поясом пользователя.
2. Смена языка и проверка перевода всех элементов WEB приложения исходя из выбранного языка.
3. Выбор номера телефона с разными кодами стран.
4. Определение местоположения пользователя и отображение соответствующего пермишена ГЕО.
5. Отображение соответствующих символов валюты.

---

## 5. Тестирование удобства использования

1. Отсутствие орфографических и грамматических ошибок, все страницы имеют корректные заголовки.
2. Выравнивание картинок, шрифтов, текстов.
3. Информативные ошибки, подсказки.
4. Подсказки существуют для всех полей.
5. Отступы между полями, колонками, рядами и сообщениями об ошибках.
6. Кнопки имеют стандартный размер, цвет.
7. На сайте нет битых ссылок и изображений.
8. Неактивные поля отображаются серым цветом.
9. Проверьте сайт при разных разрешениях экрана.
10. Скролл должен появляться только тогда, когда он требуется.
11. Отображение чекбоксов и радио-кнопок, кнопки должны быть доступны с клавиатуры, и пользователь должен быть в состоянии пользоваться сайтом, используя только клавиатуру.
12. Отображение выпадающих списков.
13. Длинный текст скрывается под многоточие.
14. Корректный выбор даты.
15. Наличие плейсхолдеров в полях.
16. Логотип ведет на главную страницу сайта.
17. Переходы и навигация между страницами и разделами меню.
18. Форма курсора меняется при наведении
19. Анимации

---

## 6. Кросс-платформенное тестирование

1. Тестирование в различных браузерах (Firefox, Chrome, Safari — это минимальный набор): анимация, верстка, шрифты, уведомления и т.д.
2. Тестирование в различных версиях ОС: Windows, Mac, Linux.
3. Java Script код работает в разных браузерах.
4. Просмотр на мобильных устройствах.

---

- внешние ссылки в новой вкладке
- фавикон и тайтл
- шеринг
- вперед/назад с помощью конпок браузера
- редирект на главную / 404 если ошибочный урл
- логи в консоли отключены [[Check-list for Security testing | see about Security testing]]
- гугл пейдж спид не ниже 70 [[Check-list for Perfomance testing | see about Perfomance]]
- соотвествие макетам
- изменение расширения экрана [[Check-list for Accessibility testing | see about Accessibility]]
- отправка форм только если все обязательные поля заполнены
- вывод ошибок валидации
- регистрация (в т.ч. через соцсети)
- валидация (в т.ч. через соцсети)

[list the most common weaknes](https://cwe.mitre.org/ "https://cwe.mitre.org/")
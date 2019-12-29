# Что произойдет если вбить в браузерную строку google.com и нажать enter?
***
Акторы:
- Пользователь
- Браузер
- Cервер
***
Цель
* Пользователь хочет получить контент веб-страницы
***
Предусловия
* Пользователь открыл браузер
***
Сценарий
***
1) Пользватель вводит google.com в адресную строку своего браузера.
2) Браузер проверяет кэш DNS-записи, чтобы найти соответствующий IP-адрес google.com.
3) Браузер инициирует TCP-соединение с сервером.
4) Браузер отправляет HTTP-запрос на веб-сервер.
5) Сервер обрабатывает запрос и отправляет ответ.
6) Сервер отправляет ответ HTTP.
7) Браузер отображает HTML-контент
 ***
 Результат
***
- Пользователь получил содержимое веб-страницы google.com
***
Исключения
***
1. Пустой запрос
2. Неверно введен запрос

![Activity diagram](https://github.com/mai-re-course/uc-univercity-chat-IvanRudko/blob/master/ActivityDiagram.png)
![Sequence diagram](https://github.com/mai-re-course/uc-univercity-chat-IvanRudko/blob/master/SequenceDiagram.png)
![Component diagram](https://github.com/mai-re-course/uc-univercity-chat-IvanRudko/blob/master/ComponentDiagram.png)

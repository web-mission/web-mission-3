# Mission 2

## Part 0



## Part1

- Вопрос 1
  
SSH — это защищённый протокол, который обеспечивает защищённое соединение с удалённым сервером. SSH используется для безопасного управления серверами, передачи файлов и других задач, требующих удалённого доступа.

- Вопрос 2
  
Нужно добавить публичный ключ в файл ~/.ssh/authorized_keys на сервере.

- Вопрос 3
 
Long polling означает, что grammY заранее отправляет запрос в Telegram с просьбой о новых обновлениях. Если сообщений нет, Telegram будет поддерживать соединение открытым до тех пор, пока не поступят новые сообщения, а затем ответит на запрос этими новыми сообщениями.

Настройка webhook означает, что вы предоставите Telegram URL-адрес, доступный из общедоступного Интернета. Когда вашему боту будет отправлено новое сообщение, Telegram возьмет на себя инициативу и отправит запрос с объектом обновления на ваш сервер.

- Вопрос 4

Issues на GitHub — это система отслеживания ошибок и запросов на улучшение проекта. Она позволяет пользователям сообщать о проблемах, задавать вопросы и предлагать новые функции для проекта.

Bootstrap — набор готовых блоков для создания веб-сайтов и приложений.
https://github.com/twbs/bootstrap/issues

React — библиотека для создания пользовательских интерфейсов
https://github.com/facebook/react/issues

- Вопрос 5

Для того чтобы Git начал отслеживать изменения в пустой папке, необходимо добавить в неё файл или создать файл с нулевым размером.

Это можно сделать с помощью команды touch:

touch path/to/folder/file

После этого Git начнёт отслеживать изменения в файле и, соответственно, в папке. 


# Mission 3

## Part 0,1,2

ссылки на скринкасты https://drive.google.com/file/d/1ybDAS4DTawLr-ut2yhJfVhbmICvgScaV/view?usp=sharing

## Part 3

1. SELECT (username) from users;

2. SELECT users.username, COUNT(messages.text) FROM users JOIN messages ON users.id = messages.from GROUP BY users.username;

3. SELECT users.username, COUNT(messages.text) As numberofreceivedmessages FROM users JOIN messages ON users.id = messages.from GROUP BY users.username order by numberofreceivedmessages DESC LIMIT 1;

4. SELECT users.username, AVG(COUNT(messages.text)) FROM users JOIN messages ON users.id = messages.to GROUP BY users.username;

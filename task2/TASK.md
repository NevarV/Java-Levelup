# Задание
Переделать программу из первого задания в клиент-серверный чат. В нем могут общаться два случайных человека. 
После регистрации пользватель помещается в очередь и ждет следующего подключившегося пользователя, после чего между ними создается чат, где могут общаться только они. 
Приложение должно быть построенная на Socket API.
Консольный клиент содержит следующие команды:
+ Просто текст — отправить сообщение собесднику (если пользователь находится в режиме ожидания собеседника и пишет в чат, то после подключения собеседник должен получить эти сообщения)
+ /reg USERNAME — регистрация (без этой команды остальной функционал недоступен)
+ /exit — выход из приложения (После выхода должен быть уведомлен и заново помещен в режим ожидания собеседник)
+ /skip [ОПЦИОНАЛЬНО] - Перейти к другому собеседнику
+ /sendFile FILENAME [ОПЦИОНАЛЬНО] - Отправить файл собеседнику (Желательно, чтобы собеседник имел возможность принять или отменить файл)


**Пример работы:**
```
» /reg Alex
Привет, Alex! Вы помещены в очередь.
» Джава — круто
[Alex]: Джава — круто
К Вам подключился Bob.
[Bob]: Согласен, джава - круто
» /exit
Пока, Alex. Приходи еще 
``Process finished with exit code 0``
```

Полезные материалы: [ссылка](MATERIALS.md)
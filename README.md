### Задача:
Чтобы привлечь новых пользователей, маркетологи хотят разместить на сторонних сайтах рекламу сообществ с высокой активностью. Нужно определить группы, в которых начала общаться большая часть их участников. В терминологии маркетинга их бы назвали пабликами с высокой конверсией в первое сообщение.

### Неоходимо

1. Перенести из S3 в staging-слой новые данные о входе и выходе пользователей из групп — файл group_log.csv.
2. Создать в слое постоянного хранения таблицы для новых данных.
3. Перенести новые данные из staging-области в слой DDS.
4. Рассчитать конверсионные показатели для десяти самых старых групп:
* количество пользователей, вступивших в группу, — cnt_added_users;
* количество участников группы, которые написали хотя бы одно сообщение, — * cnt_users_in_group_with_messages;
* конверсию в первое сообщение из вступления в группу — group_conversion.


### Использованные инструменты

Python, PostgreSQL, Pandas , Airflow, Vertica, S3, json

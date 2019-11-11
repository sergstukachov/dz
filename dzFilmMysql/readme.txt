Создано три таблицы actor , film , producer. Между таблицами film and producer создана связь один ко многим. Для связи многие ко многим между actir and film создана четвертая таблица actor_film.

mysql> select*from films;                                                       +----+--------------------------+-------------+
| id | film                     | producer_id |
+----+--------------------------+-------------+
|  1 | Pirates of the Caribbean |           1 |
|  2 | Blood sport 2            |           2 |
|  3 | Matrix                   |           4 |
|  4 | Wanted                   |           3 |
|  5 | Night Dozor              |           3 |
|  6 | Jon Uik                  |           5 |
+----+--------------------------+-------------+
6 rows in set (0.00 sec)

mysql> select*from actors;
+----+----------------------+
| id | actor                |
+----+----------------------+
|  1 | John Depp            |
|  2 | Van Damme            |
|  3 | Konstantin Habenskiy |
|  4 | Angelina Joli        |
|  5 | Morgan Frimen        |
|  6 | Kianu Reevs          |
+----+----------------------+
6 rows in set (0.01 sec)

mysql> select*from producer;
+----+----------------+
| id | producer       |
+----+----------------+
|  1 | Rob Marshal    |
|  2 | Jeff Schechter |
|  3 | Becmanbecov    |
|  4 | Wachowski      |
|  5 | Chad Stahelski |
+----+----------------+
5 rows in set (0.00 sec)

mysql> select*from actor_film;
+----------+---------+
| actor_id | film_id |
+----------+---------+
|        1 |       1 |
|        2 |       2 |
|        3 |       4 |
|        3 |       5 |
|        4 |       4 |
|        5 |       4 |
|        6 |       3 |
|        6 |       6 |
+----------+---------+
8 rows in set (0.00 sec)

mysql> 


1) Разработать REST API для простого сервиса управления задачами. Должны быть реализованы следующие эндпоинты: (Сделано)

-Создание задачи
-Получение списка всех задач
-Обновление задачи
-Удаление задачи
-Получение задачи по ID


2) Подключите реляционную базу данных H2 к вашему проекту. (Сделано) (Модель создание таблиц в БД - в оперативной памяти) (Сделано)

Запрос для создания таблицы

CREATE TABLE TASKS (
    ID BIGINT AUTO_INCREMENT PRIMARY KEY,
    TASK_NAME VARCHAR(255) NOT NULL,
    DESCRIPTION TEXT,
    STATUS VARCHAR(64),
    CREATE_AT TIMESTAMP DEFAULT CURRENT_TIMESTAMP(),
    UPDATE_AT TIMESTAMP DEFAULT CURRENT_TIMESTAMP()
)



3) Реализуйте логирование запросов и ответов которые проходят через ваш сервис. (Сделано)

Дополнительные задания (+1 к каждой при выполнении)

1) Из вашего проекта сделать http запрос (GET) на адрес: https://api.restful-api.dev/objects  Полученный ответ залогировать.(Сделано)

2) Напишите unit-тесты для crud методов в вашем service классе для управления задачами.(Сделано)

3) Реализуйте отправку созданных задач на email. Можно использовать готовую библиотеку для отправки почты. (Сделано)

4) Добавьте Basic Authentication для защиты API.(Сделано)

5) Реализуйте кэширование "Получение списка всех задач" с использованием Redis. (Сделано)

6) Напишите dockerfile для вашего проекта (Сделано)

В проекте использовал Java, Spring Boot, Hibernate, Redis, Docker. 
Для запросов использовал Postman

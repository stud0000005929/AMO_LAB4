Описание проекта
В рамках этого проекта была создана система обработки данных с применением Apache Airflow. Основные этапы, выполненные в ходе работы:
1.	Применение Docker:
•	Для развертывания Apache Airflow использовался Docker, что упростило управление окружением и зависимостями.
•	Docker-контейнеры обеспечили изоляцию и повторяемость среды, что облегчило развертывание и масштабирование системы.
•	Были настроены Docker Compose файлы для автоматизации запуска и управления контейнерами.
2.	Разработка DAG:
•	Был реализован Directed Acyclic Graph (DAG), который выполняет следующие задачи:
•	Генерация 100 текстовых файлов с случайными латинскими символами.
•	Подсчет количества вхождений символа "a" в каждом файле.
•	Суммирование результатов подсчета для всех файлов.
•	DAG был написан на Python с использованием библиотеки Airflow для определения задач и их зависимостей.
•	Включены механизмы обработки ошибок и повторных попыток для повышения надежности выполнения задач.
3.	Тестирование:
•	Проведено тестирование DAG в интерфейсе Airflow для проверки корректности выполнения задач.
•	Были выполнены unit-тесты для отдельных компонентов DAG, чтобы убедиться в их корректной работе.
•	Включены интеграционные тесты для проверки взаимодействия между различными задачами в DAG.
•	Использовались мониторинговые инструменты Airflow для отслеживания состояния выполнения задач и выявления возможных проблем.

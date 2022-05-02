﻿# Stepik_ML_contest
## Задание
Используя RandomForestClassifier предсказать, сможет ли пользователь успешно закончить онлайн курс. Проверка точности предсказания выполнялась с помощью ROC AUC score.
## Данные:
**events_train.csv** - данные о действиях, которые совершают студенты со стэпами:
- step_id - id стэпа;
- user_id - анонимизированный id юзера;
- timestamp - время наступления события в формате unix date;
- action - событие, возможные значения: 
    - discovered - пользователь перешел на стэп;
    - viewed - просмотр шага;
    - started_attempt - начало попытки решить шаг, ранее нужно было явно нажать на кнопку - начать решение, перед тем как приступить к решению практического шага;
    - passed - удачное решение практического шага.

**submissions_train.csv** - данные о времени и статусах сабмитов к практическим заданиям:
- step_id - id стэпа
- timestamp - время отправки решения в формате unix date
- submission_status - статус решения
- user_id - анонимизированный id юзера
В данных **submission_data_test.csv** и **events_data_test.csv**хранится информация о решениях и действиях для 6184 студентов за первые два дня прохождения курса. Это 6184 студентов, которые проходили курс в период с мая 2018 по январь 2019
**Результат модели на тестовой выборке - 0.8902**

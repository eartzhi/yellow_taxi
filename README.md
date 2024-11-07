# New York City Taxi Trip Duration. PROJECT-5. Задача регрессии

## Оглавление   
[1. Описание проекта](#оглавление)  
[2. Какой кейс решаем?](#какой-кейс-решаем)  
[3. Краткая информация о данных](#краткая-информация-о-данных)  
[4. Этапы работы над проектом](#этапы-работы-над-проектом)  
[5. Результат](#результаты)    

### Описание проекта    
Проект №5 курса DSPR Skillfsctory 2024 года.

Файл learning.ipynb - итоговый расчет.

:arrow_up:[к оглавлению](#оглавление)


### Какой кейс решаем?    
In this competition, Kaggle is challenging you to build a model that predicts the total ride duration of taxi trips in New York City. Your primary dataset is one released by the NYC Taxi and Limousine Commission, which includes pickup time, geo-coordinates, number of passengers, and several other variables.

Longtime Kagglers will recognize that this competition objective is similar to the ECML/PKDD trip time challenge we hosted in 2015. But, this challenge comes with a twist. Instead of awarding prizes to the top finishers on the leaderboard, this playground competition was created to reward collaboration and collective learning.

We are encouraging you (with cash prizes!) to publish additional training data that other participants can use for their predictions. We also have designated bi-weekly and final prizes to reward authors of kernels that are particularly insightful or valuable to the community.

**Метрика качества**     
В качестве критерия качества модели в соревновании выбрана метрики:
Median Absolute Error (MeAE), показывает медианную абсолютную ошибку предсказанных значений от фактических.
Root Mean squered Log Error (RMSLE), показывает вычисленный корень из квадратичной ошибки в логарифмическом масштабе предсказанных значений от фактических.
.

**Что практикуем**     
Практикуем решение реальных задачь с помощью машинного обучения.


### Краткая информация о данных

[Данные](https://drive.google.com/drive/folders/1J6rbtpvFTBgKOm5OWxB4O4zcnPXgcUFd?usp=sharing "Если ссылка недоступна, прошу писать на личную почту").
Данные о клиенте и таксопарке:

id — уникальный идентификатор поездки;
vendor_id — уникальный идентификатор поставщика услуг (таксопарка), связанного с записью поездки.
Временные характеристики:

pickup_datetime — дата и время, когда был включён счётчик поездки;
dropoff_datetime — дата и время, когда счётчик был отключён.
Географическая информация:

pickup_longitude — долгота, на которой был включён счётчик;
pickup_latitude — широта, на которой был включён счётчик;
dropoff_longitude — долгота, на которой счётчик был отключён;
dropoff_latitude — широта, на которой счётчик был отключён.
Прочие признаки:

passenger_count — количество пассажиров в транспортном средстве (введённое водителем значение);
store_and_fwd_flag — флаг, который указывает, сохранилась ли запись о поездке в памяти транспортного средства перед отправкой поставщику (Y — хранить и пересылать, N — не хранить и не пересылать поездку).
Целевой признак:

trip_duration — продолжительность поездки в секундах.

:arrow_up:[к оглавлению](#оглавление)

### Этапы работы над проектом  
Работа разбита на 6 этапов:

1. Постановка задачи
2. Знакомство с данными, базовый анализ и расширение данных
3. Разведывательный анализ данных (EDA)
4. Отбор и преобразование признаков
5. Решение задачи регрессии: линейная регрессия и деревья решений
6. Решение задачи регрессии: ансамблевые методы и построение прогноза


:arrow_up:[к оглавлению](#оглавление)


### Результаты:  
*Наилучшие результаты на данном наборе данных показывает модель GradientBoostingRegressor.*  
*На валидационной выборке модель показала:*  
*RMSLE: 0.40*  
*MeAE: 1.8*  

:arrow_up:[к оглавлению](#оглавление)

# Project_Hyper_params

____
### О проекте
Подбор гиперпараметров для модели логистической регрессии и случайный лес.

### Какая задача решается
Необходимо предсказать биологический ответ молекул (столбец 'Activity') по их химическому составу (столбцы D1-D1776).

Техническая задача: определить гиперпараметры, которые позволят осуществлять наилучшее предсказание, ключевая метрика качества подбора гиперпараметров F-1

### Краткая информация о данных
Представлены предобработанные данные по химическим молекулам.

### Этапы работы над проектом
1. Обучение моделей логистической регрессии и случайный лес с дефолтными параметрами.
2. Проведена оптимизация гиперпараметров методом GridSearchCV для обоих моделей. 
3. Проведена оптимизация гиперпараметров методом RandomizedSearchCV для обоих моделей.
4. Проведена оптимизация гиперпараметров методом Hyperopt для обоих моделей.
5. Проведена оптимизация гиперпараметров методом Optuna для обоих моделей.
  
### Результаты
1. Подбор гиперпараметров методом GridSearchCV для модели Логистической регрессии незначительно увеличил F-1 с 0,78 до 0,79 при значительном увеличении времени.
  Подбор гиперпараметров методом GridSearchCV для модели Случайный лес не изменил F-1, при значительном увеличении времени.
2. Подбор гиперпараметров методом RandomizedSearchCV для модели Логистической регрессии незначительно увеличил F-1 с 0,78 до 0,79. Затраченное время минимально.
  Подбор гиперпараметров методом RandomizedSearchCV для модели Случайный лес не изменил F-1. Затраченное время минимально.
3. Подбор гиперпараметров методом Hyperopt для модели Логистической регрессии незначительно увеличил F-1 с 0,78 до 0,79. Времени затрачено незначительное количество.
  Подбор гиперпараметров методом Hyperopt для модели Слйчайный лес незначительно увеличил F-1 с 0,80 до 0,81.
 4. Подбор гиперпараметров методом Optuna для модели Логистической регрессии незначительно увеличил F-1 с 0,78 до 0,79. Затрачено значительное количество времени
  Подбор гиперпараметров методом Optuna для модели Слйчайный лес незначительно увеличил F-1 с 0,80 до 0,81. Затрачено незначительное количество времени.

### Выводы
Проведенный анализ подбора гиперпараметров для двух моделей машинного обучения различными методами показал, что наилучшие результаты показала модель Случайный лес. Способы Optuna и Hyperopt показали сопоставимые результаты, так как удалось поднять  F-1 c 0.80  до 0.81. 


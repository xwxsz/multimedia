# Лабораторные работы по дисциплине "Методы, средства и технологии мультимедиа"
**Студент:** Шуленков Илья <br/>
**Группа:** М8О-406Б-21 <br/>
<br/>
# Выбор наборов данных 
Для задачи классификации был выбран датасет [Video Games Rating By 'ESRB'](https://www.kaggle.com/datasets/imohtn/video-games-rating-by-esrb?resource=download) <br/>
Цель: определить возрастной рейтинг игры на основе ее характеристик <br/>
<br/>
Для задачи регресии был выбран датасет [Real Estate Valuation Taiwan](https://archive.ics.uci.edu/dataset/477/real+estate+valuation+data+set) <br/>
Цель: определить цену недвижимости на основе различных характеристик <br/>
<br/>
# Выбор метрик
Задача классификации <br/>
| Метрика | Описание |
| --- | --- |
| Accuracy | Доля верных предсказаний от общего числа предсказаний|
| F1 | Гармоническое среднее между точностью и полнотой модели |

Задача регрессии 
| Метрика | Описание |
| --- | --- |
| MAE | Cреднее абсолютное отклонение предсказанных значений от реальных значений |
| R^2 | Коэффициент детерминации показывает, насколько хорошо модель объясняет вариацию данных |

# ЛР1 (KNN)

| Задача | Модель | Accuracy | F1 | MAE | R^2 |
| -- | -- | -- | -- | -- | -- |
| Классификация | Бейзлайн | 0.8047 | 0.8025 |  |  |
|  | Улучшенный бейзлайн | 0.8285 | 0.8272 |  |  |
|  | Самостоятельная имплементация | 0.8127 | 0.8121 |  |  |
| Регрессия | Бейзлайн |  |  | 6.103 | 0.6115 |
|  | Улучшенный бейзлайн |  |  | 5.077 | 0.7112 |
|  | Самостоятельная имплементация |  |  | 4.980 | 0.7118 |

# ЛР2 (Линейные модели)

| Задача | Модель | Accuracy | F1 | MAE | R^2 |
| -- | -- | -- | -- | -- | -- |
| Классификация | Бейзлайн | 0.8681 | 0.8704 |  |  |
|  | Улучшенный бейзлайн | 0.8734 | 0.8754 |  |  |
|  | Самостоятельная имплементация | 0.8760 | 0.8767 |  |  |
| Регрессия | Бейзлайн |  |  | 5.418 | 0.6745 |
|  | Улучшенный бейзлайн |  |  | 4.794 | 0.7497 |
|  | Самостоятельная имплементация |  |  | 4.856 | 0.7415 |

# ЛР3 (Решающее дерево)

| Задача | Модель | Accuracy | F1 | MAE | R^2 |
| -- | -- | -- | -- | -- | -- |
| Классификация | Бейзлайн | 0.8179 | 0.8180 |  |  |
|  | Улучшенный бейзлайн | 0.8285 | 0.8296 |  |  |
|  | Самостоятельная имплементация | 0.8281 | 0.8295 |  |  |
| Регрессия | Бейзлайн |  |  | 5.360 | 0.6787 |
|  | Улучшенный бейзлайн |  |  | 4.719 | 0.7512 |
|  | Самостоятельная имплементация |  |  | 4.597 | 0.7472 |

# ЛР4 (Случайный лес)

| Задача | Модель | Accuracy | F1 | MAE | R^2 |
| -- | -- | -- | -- | -- | -- |
| Классификация | Бейзлайн | 0.8443 | 0.8453 |  |  |
|  | Улучшенный бейзлайн | 0.8522 | 0.8530 |  |  |
|  | Самостоятельная имплементация | 0.7995 | 0.8009 |  |  |
| Регрессия | Бейзлайн |  |  | 3.879 | 0.8101 |
|  | Улучшенный бейзлайн |  |  | 3.611 | 0.8291 |
|  | Самостоятельная имплементация |  |  | 3.694 | 0.8094 |

# ЛР5 (Градиентный бустинг)

| Задача | Модель | Accuracy | F1 | MAE | R^2 |
| -- | -- | -- | -- | -- | -- |
| Классификация | Бейзлайн | 0.8575 | 0.8579 |  |  |
|  | Улучшенный бейзлайн | 0.8628 | 0.8646 |  |  |
|  | Самостоятельная имплементация | 0.8259 | 0.8284 |  |  |
| Регрессия | Бейзлайн |  |  | 4.083 | 0.7799 |
|  | Улучшенный бейзлайн |  |  | 3.935 | 0.8004 |
|  | Самостоятельная имплементация |  |  | 3.935 | 0.7919 |

# Вывод

Лучший алгоритм для задачи регрессии - случайный лес с улучшенным бейзлайном (хотя и собственная имплементация показала неплохие результаты) <br/>
<br/>
Лучшим же алгоритмом для задачи классификации стала самостоятельная реализация логистической регрессии, которая показала наилучщие результаты, что может быть связано с тем, что данные в датасете линейно разделимы <br/>
Почти также хорошо себя показал градиентный бустинг с улучшенным бейзлайном 




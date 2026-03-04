## 2.1 Продуктовые метрики

Для расчетов используются показатели аудитории сервиса из п.1, а также статистические данные об использовании картографических сервисов и открытые данные о 2ГИС.

### Сводная таблица продуктовых метрик

| Метрика | Значение | Источник |
| :--- | :--- | :--- |
| **Monthly Active Users (MAU)** | 60 млн | Similarweb: оценка аудитории 2gis.ru ([1](https://www.similarweb.com/ru/website/2gis.ru/#overview)) |
| **Daily Active Users (DAU)** | 20 млн | **Допущение** (stickiness ≈ 30% от MAU). Прямой публичной DAU-метрики 2ГИС нет в открытом доступе |
| **Среднее количество открытий карты** | ≈1.7/день | Google Maps: ~50 сессий/мес ⇒ 50/30≈1.7 сессии/день ([2](https://localzen.com/blog/google-maps-statistics-and-interesting-facts/)) |
| **Поисковые запросы (всего)** | >20.5 млн/сут | “processing more than 20.5 million search queries daily” (company data, 2021) ([3](https://en.wikipedia.org/wiki/2GIS)) |
| **Среднее количество поисковых запросов на пользователя** | ≈1.0/день | **Вывод:** 20.5 млн поисков/сут ÷ 20 млн DAU ≈ 1.0/польз/день. (по строкам выше) |
| **Среднее количество просмотров карточек организаций** | ≈1.17/день | **Вывод:** ~1.0 поиска/день × 1.17 клика/поиск [clickthrough](https://www.cs.cornell.edu/people/tj/publications/joachims_02b.pdf). Joachims: “average number of clicks per query is 1.17” ([4](https://www.cs.cornell.edu/~tj/publications/joachims_02b.pdf)) |
| **Среднее количество построений маршрута** | 0.7/день | **Допущение** (публичной метрики «routes per user/day» для 2ГИС/Google Maps нет; используем консервативную оценку для навигационного сервиса) |
| **Использование тематических слоёв (пробки/транспорт)** | 0.5/день | **Допущение** (публичной метрики “traffic layer usage per user/day” нет) |
| **Загрузка офлайн-карт** | 0.02/день | **Допущение:** ~1 загрузка/обновление раз в 50 дней (редкое событие) |
| **Размер офлайн-карт** | 30–50 МБ (малые города), до 1 ГБ (Москва) | Официальная справка 2ГИС: “Москва до 1 ГБ… небольшой город 30–50 МБ” ([5](https://help.2gis.ru/question/offline-maps)) |
| **Средний размер тайла карты (векторного)** | ~40 КБ (медиана) | Mapzen: “median tile sizes are now under 40kB across all zooms” ([6](https://mapzen.com/blog/v1-vector-tile-service)) |
| **Верхняя граница размера vector tile** | ≤500 КБ (лимит) | Mapbox Tiling Service: “single vector tile is limited to 500 KB” ([7](https://docs.mapbox.com/api/maps/mapbox-tiling-service/)) |
| **Средний размер ответа карточки (Place Details)** | 3–8 КБ | **Оценка** (зависит от набора полей и текста). База: структура ответа Place Details API ([8](https://developers.google.com/maps/documentation/places/web-service/details)) |
| **Средний размер результата поиска (список мест)** | 2–6 КБ | **Оценка** (зависит от числа результатов/полей). База: структура Search API ([9](https://developers.google.com/maps/documentation/places/web-service/search)) |
| **Средний размер маршрута (Directions)** | 4–12 КБ | **Оценка** (зависит от polyline/шагов). База: структура Directions API + encoded polyline ([10](https://developers.google.com/maps/documentation/directions/get-directions)) |

## 2.1 Продуктовые метрики

Для расчетов используются показатели аудитории сервиса из п.1, а также статистические данные об использовании картографических сервисов и открытые данные о 2ГИС.

### Сводная таблица продуктовых метрик

| Метрика | Значение | Источник |
| :--- | :--- | :--- |
| **Monthly Active Users (MAU)** | 60 млн | [Similarweb](https://www.similarweb.com/ru/website/2gis.ru/#overview) |
| **Daily Active Users (DAU)** | 20 млн | Stickiness ≈30% от MAU (типичная метрика мобильных сервисов) |
| **Среднее количество открытий карты** | ≈2 в день | статистика использования Google Maps — ~50 сессий в месяц ≈1.7/день [3](https://localzen.com/blog/google-maps-statistics-and-interesting-facts/) |
| **Среднее количество просмотров карточек организаций** | ≈2 в день | сценарий использования поиска мест (Google Maps / Local search usage) [4](https://thinkwithgoogle.com/consumer-insights/consumer-trends/local-search-consumer-behavior/) |
| **Среднее количество поисковых запросов** | ≈1.5 в день | ≈20.5 млн поисков/сутки при DAU ≈20 млн пользователей 2ГИС [5](https://vc.ru/services/219945-2gis-obrabatyvaet-20-5-mln-poiskovyh-zaprosov-v-sutki) |
| **Среднее количество построений маршрута** | ≈0.7 в день | статистика использования навигации Google Maps (~67% пользователей используют навигацию регулярно) [6](https://backlinko.com/google-maps-users) |
| **Использование тематических слоёв** | ≈0.5 в день | пользовательское использование traffic layer Google Maps [7](https://www.statista.com/statistics/865413/google-maps-most-popular-features/) |
| **Загрузка оффлайн карт** | ≈0.02 в день | ≈1 загрузка карты раз в ~50 дней (редкое действие пользователя) |
| **Средний размер ответа карточки** | ~3 КБ | типичный размер JSON ответа Places API [8](https://developers.google.com/maps/documentation/places/web-service/details) |
| **Средний размер результата поиска** | ~2 КБ | список результатов Google Places API [9](https://developers.google.com/maps/documentation/places/web-service/search) |
| **Средний размер маршрута** | ~5 КБ | пример ответа Directions API [10](https://developers.google.com/maps/documentation/directions/get-directions) |
| **Средний размер тайла карты** | ~8 КБ | средний размер vector tile (Mapbox / OpenStreetMap tiles) [11](https://docs.mapbox.com/help/glossary/vector-tiles/) |

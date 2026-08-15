# TLC High Volume FHV Trip Record Data

Данные [NYC Taxi & Limousine Commission](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page) о поездках крупных сервисов заказа автомобилей, включая Uber и Lyft, за январь 2025 — апрель 2026 года. В проекте используются 16 ежемесячных файлов `fhvhv_tripdata_*.parquet`; одна строка соответствует одной поездке.

## High Volume FHV

| Поле | Описание |
|---|---|
| `hvfhs_license_num` | Лицензия оператора HVFHS |
| `dispatching_base_num` | База, отправившая автомобиль |
| `originating_base_num` | База, изначально принявшая заказ |
| `request_datetime` | Время получения заказа |
| `on_scene_datetime` | Время прибытия автомобиля к месту посадки |
| `pickup_datetime` | Время начала поездки |
| `dropoff_datetime` | Время окончания поездки |
| `PULocationID` | TLC-зона посадки |
| `DOLocationID` | TLC-зона высадки |
| `trip_miles` | Расстояние поездки, мили |
| `trip_time` | Продолжительность поездки, секунды |
| `base_passenger_fare` | Базовая стоимость без налогов, сборов и чаевых |
| `tolls` | Сумма платы за платные дороги |
| `bcf` | Взнос в Black Car Fund |
| `sales_tax` | Налог с продаж |
| `congestion_surcharge` | Сбор за загруженность |
| `airport_fee` | Аэропортовый сбор |
| `tips` | Чаевые |
| `driver_pay` | Выплата водителю без чаевых и дорожных сборов |
| `shared_request_flag` | Признак запроса совместной поездки |
| `shared_match_flag` | Признак фактического совпадения совместной поездки |
| `access_a_ride_flag` | Поездка по программе MTA Access-A-Ride |
| `wav_request_flag` | Признак запроса автомобиля, доступного для коляски |
| `wav_match_flag` | Признак фактического предоставления автомобиля, доступного для коляски |
| `cbd_congestion_fee` | Сбор за поездку в зоне платного въезда в деловой центр Манхэттена |

[Официальный словарь High Volume FHV](https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_hvfhs.pdf)

`PULocationID` и `DOLocationID` расшифровываются через [Taxi Zone Lookup Table](https://d37ci6vzurychx.cloudfront.net/misc/taxi_zone_lookup.csv).

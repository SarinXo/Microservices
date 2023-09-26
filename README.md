# microservices
---------------------------------------------------------------------------------------------
#                                        controllers                                        #
---------------------------------------------------------------------------------------------


----------------------------------------person-service---------------------------------------

Получить список пользователей

[GET]http://localhost:17957/person-service/persons

Получить конкретного пользователя по id

[GET]http://localhost:17957/person-service/persons/{id}

Зарегистрировать пользователя в базе данных

[POST]http://localhost:17957/person-service/persons

Получить блок Weather (Main) от person с {id} по его локации

[GET]http://localhost:17957/person-service/persons/{id}/weather

Получить id сервиса к которому был осуществлен запрос

[GET]http://localhost:17957/person-service/service/id


----------------------------------------wether-service---------------------------------------

получить погоду по координатам

[GET]http://localhost:17957/weather-service/weather/lat={{lat}}&lon={{lon}}

получить блок погоды по координатам

[GET]http://localhost:17957/weather-service/weather/lat={{lat}}&lon={{lon}}/main


--------------------------------------location-service---------------------------------------

Получить геоданные по названию города

[GET]http://localhost:17957/location-service/geodata?location={location}

Зарегистрировать в базе данных город с координатами

[POST]http://localhost:17957/location-service/geodata

Получить погоду по ЗАРЕГИСТРИРОВАННОМУ названию города

[GET]http://localhost:17957/location-service/weather?location={location}

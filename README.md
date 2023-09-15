# microservices
---------------------------------------------------------------------------------------------
#                                        controllers                                        #
---------------------------------------------------------------------------------------------


----------------------------------------person-service---------------------------------------

Получить список пользователей

[GET]http://localhost:8088/person-service/persons

Получить конкретного пользователя по id

[GET]http://localhost:8088/person-service/persons/{id}

Зарегистрировать пользователя в базе данных

[POST]http://localhost:8088/person-service/persons


----------------------------------------wether-service---------------------------------------

получить погоду по координатам

[GET]http://localhost:8088/weather-service/weather/lat={{lat}}&lon={{lon}}

получить блок погоды по координатам

[GET]http://localhost:8088/weather-service/weather/lat={{lat}}&lon={{lon}}/main


--------------------------------------location-service---------------------------------------

Получить геоданные по названию города

[GET]http://localhost:8088/location-service/geodata?location={location}

Зарегистрировать в базе данных город с координатами

[POST]http://localhost:8088/location-service/geodata

Получить погоду по ЗАРЕГИСТРИРОВАННОМУ названию города

[GET]http://localhost:8088/location-service/weather?location={location}

# Juli_Ivantsova_Test1_junior1# Juli_IvantSova_Task_1_Junior

Проверка проекта в Postman.
по ссылке
GET
http://localhost:8080/allCity
получаем все города. В Кеш они не попадают.
GET
http://localhost:8080/city?name=Gomel
http://localhost:8080/city?name=Minsk
Отправляем два города в Кеш
GET
http://localhost:8080/cache?name=city-zip-cache
Проверяем Кеш, там два города
Gomel и Minsk

Post
http://localhost:8080/city
{
"cityName": "TRTYU",
"zipCode":"566987"
}
{
"cityName": "Polotck",
"zipCode":"5667678"
}
Добавляем два города в коллекцию и Кеш
Get
http://localhost:8080/cache?name=city-zip-cache
Проверяем, что вновь добавленные города в кеше

Delete
http://localhost:8080/cache?name=Braslav
удаляем город из таблицы и Кеш

Delete
Чистить только Кеш целиком.
http://localhost:8080/delete?name=Minsk



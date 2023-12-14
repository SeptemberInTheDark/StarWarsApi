# StarWarsApi
```Requests from api

Что нужно сделать
Изучите документацию бесплатного стороннего сервиса The Star Wars API: SWAPI.

Обратите внимание на доступные ресурсы (категории данных) и на то, как организован поиск (раздел Searching). Мы будем делать поиск только по ресурсу people.

Как обычно, ваша программа — это npm-модуль в папке проекта (05_async в вашем репозитории), все её зависимости должны быть указаны в файле package.json (см. прошлые модули, если нужно освежить установку зависимостей).

Ваша программа принимает в командной строке один или более поисковых запросов:

node index.js r2 skywalker xyz "Padmé Amidala"
Обратите внимание, тут передано четыре аргумента, последний — "Padmé Amidala" — заключён в кавычки, потому что содержит пробел.

Если программа не получила ни одного аргумента, она должна напечатать предупреждение и завершить работу.

Для каждого аргумента нужно выполнить соответствующий HTTP-запрос для поиска по ресурсу people. Этот запрос может вернуть ноль или более персонажей, возможно, больше одного.

Все запросы должны выполняться параллельно.

Если какой-то запрос выполнился с ошибкой, программа должна:

вывести ошибку в консоль,

считать, что запрос вернул ноль записей, и продолжить работу.

Если какой-то запрос выполнился успешно, но никого не найдено (вернул ноль записей), программа должна вывести предупреждение “No results found for ‘<поисковый аргумент>’”.

В конце программы нужно собрать всех найденных персонажей и вывести о них следующую информацию:

Total results: 5.

All: Anakin Skywalker, Luke Skywalker, Padmé Amidala, R2-D2, Shmi Skywalker.

Min height: R2-D2, 92 cm.

Max height: Anakin Skywalker, 188 cm.
Имена во второй строчке должны идти в алфавитном порядке. 

Если все запросы вместе вернули ноль персонажей, предыдущую информацию выводить не нужно.
```

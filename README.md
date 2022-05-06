# Task2
Кэширующий DNS сервер

Сервер получает от клиента запрос и выполняет его разрешение.<br>
Получив ответ от старшего сервера, разбирает пакет и извлекает из него информацию обо всех полях. <br>
Полученная информация записывается в кэш и при повторном запросе от клиента сервер возвращает необходимую информацию уже из кэша. <br>
При этом кэш регулярно обновляется: из него удаляются "просроченные" записи.

## Применение
Запустить сервер можно вызовом из консоли:<br>
`python dns.py`<br>
Запросы от клиента могут выглядеть следующим образом: <br>
`nslookup type=A vk.com 127.0.0.1`<br>
`nslookup type=NS ya.ru 127.0.0.1`<br>
`nslookup urfu.ru 127.0.0.1`
![Example](https://github.com/Alina200207/Task2/blob/master/animation%20(2).gif)

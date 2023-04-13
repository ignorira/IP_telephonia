Faculty: ICT

Course: Network programming

Year: 2023

Group: K34212

Автор: Сорокина Ирина Игоревна

Lab: 1

***Часть 1***
**Цель:** изучить построение сети IP-телефонии с помощью маршрутизатора, коммутатора и IP телефонов.

Собираем схему соединения в среде Cisco Packet Tracer.
![image](https://user-images.githubusercontent.com/58992611/231842309-d59f3cbb-c911-4f69-9500-e838e7a6d09f.png)

Изменяем название маршрутизатора на CMERouter.
![image](https://user-images.githubusercontent.com/58992611/231842352-e94bbd5f-62cb-4e51-957c-fe18e487bb8c.png)

Отключаем синтаксис ввода слов от DNS серверов и задаем пароли для защиты маршрутизатора в удаленном и консольном режиме.
![image](https://user-images.githubusercontent.com/58992611/231842391-7893d0f1-8160-4d35-8c37-26d63b52f649.png)

Сконфигурируем интерфейс fa0/0.
![image](https://user-images.githubusercontent.com/58992611/231842440-2915fac8-f860-4065-a49a-c80ba3ea28af.png)

Для автоматической настройки компьютеров и IP-телефонов в сети надо настроим DHCP сервер на маршрутизаторе. В конфигурационном режиме создадим пул DHCP адреса с названием VOICE, а затем зададим сеть, в которой будет работать DHCP сервер. Укажем ip адрес нужного VLAN и включим опцию 150. 
Теперь настроим телефонный сервис в автоматическом режиме. В данном режиме ведется диалоговый обмен сообщениями, маршрутизатор только запрашивает необходимые параметры. Задаем максимальное количество номеров, присваиваемых IPтелефоном и автоматическое назначение внешних номеров.
![image](https://user-images.githubusercontent.com/58992611/231842494-728c799d-6d0d-44c2-9469-a9efa66998ed.png)

Настроим интерфейс управления коммутатором в сети VLAN через назначение диапазона портов.
![image](https://user-images.githubusercontent.com/58992611/231842547-fd5501af-7945-4578-bd10-b290731ea813.png)

Задаем номера телефонов и осуществляем созвон.
![image](https://user-images.githubusercontent.com/58992611/231842588-7f70ad0a-93a2-4df7-80c3-f16cb4f320ab.png)

***Часть 2***
**Цель:** изучить построение сети IP-телефонии, научиться стандартной настройке технологии VOIP.
Собираем схему соединения в среде Cisco Packet Tracer.
![image](https://user-images.githubusercontent.com/58992611/231842638-720946a7-00b6-47f2-b65e-0f339421c582.png)

Создадим vlan и присвоим им наименования.
![image](https://user-images.githubusercontent.com/58992611/231842689-faf2d641-7404-4d8e-bf6a-9800bf5478c2.png)

Настроим vlan 99 и зададим маршрут по умолчанию.
![image](https://user-images.githubusercontent.com/58992611/231842731-560bc3f0-8fbd-4be2-b293-6757fca03d13.png)
![image](https://user-images.githubusercontent.com/58992611/231842760-5aff4905-69a1-4371-b033-04894ac8c6b6.png)

Настроим интерфейс управления коммутатором в сети VLAN через назначение диапазона портов.
![image](https://user-images.githubusercontent.com/58992611/231842804-65388dfc-4a69-4f77-85ee-60840dffb63a.png)

Включаем интерфейс FastEthernet0/0:
![image](https://user-images.githubusercontent.com/58992611/231842846-960955b0-8efa-42d2-94f8-6ad18c48b5d3.png)

Создаем логический подынтерфейс для VLAN 10, VLAN 20, VLAN 99 и исключаем из пула адрес интерфейса маршрутизатора и DNS-сервера.
![image](https://user-images.githubusercontent.com/58992611/231842898-d53ac8cd-56d2-43a2-85d6-fff84bf8f164.png)

Настраиваем DHCP сервер для передачи голоса и данных на роутере и настраиваем телефонный сервис в автоматическом режиме.
![image](https://user-images.githubusercontent.com/58992611/231842940-87b7393a-2efc-4f8e-9f10-ab12f6a1a593.png)

Присваиваем номера для всех IP-телефонов в сети.
![image](https://user-images.githubusercontent.com/58992611/231842993-b00c85d7-7158-4358-b41b-cd6fd7218079.png)

Успешные пинги между устройствами.
![image](https://user-images.githubusercontent.com/58992611/231843051-697817e0-a2d4-4231-a135-6edceb86d612.png)

Результат успешного прозвона.
![image](https://user-images.githubusercontent.com/58992611/231843092-19c341c6-ae90-4589-8592-22d4bff896f4.png)

**Вывод:** в ходе выполнения лабораторной работы были получены навыки работы с IP-телефонией с помощью маршрутизатора, коммутатора и IP телефонов.

Faculty: ICT

Course: Network programming

Year: 2023

Group: K34212

Автор: Сорокина Ирина Игоревна

Lab: 3

**Цель:** изучить построение сети IP-телефонии между удаленными филиалами с помощью маршрутизаторов и коммутаторов.
Собираем схему соединения в среде Cisco Packet Tracer.
![image](https://user-images.githubusercontent.com/58992611/231866613-c3d5df76-3231-4938-aa06-1958f2c5ea18.png)

Так как между роутерами должно быть проложено DCE/DTE соединение, добавляем роутерам нужные разъемы.
![image](https://user-images.githubusercontent.com/58992611/231866686-40d27b5d-9b22-4f74-b0a9-71352b986e66.png)

В конфигурационном режиме изменим название маршрутизаторов на RouterA и RouterB:
![image](https://user-images.githubusercontent.com/58992611/231866735-56bf8b1f-c2a0-48ba-8486-534d02828dde.png)

Произведем конфигурацию интерфейса FastEthernet0/0 на маршрутизаторе RouterA.
![image](https://user-images.githubusercontent.com/58992611/231866784-e2a0d7cb-4360-49c0-83dd-92acfb2b8c65.png)

Настроим DCE порт на Router A и DTE порт на Router В.
![image](https://user-images.githubusercontent.com/58992611/231866835-099a9502-045c-4642-9dc7-538951ba63c1.png)

Настроим dhcp сервер на маршрутизаторе для автоматической настройки компьютеров и IP-телефонов в сети. В конфигурационном режиме создадим пул DHCP адреса с названием Т1, зададим сеть, в которой будет работать DHCP сервер, укажем ip адрес нужного VLAN и включим опцию 150. 
![image](https://user-images.githubusercontent.com/58992611/231866886-d3c07e3f-1d77-4cb4-b7fc-d923df78cafe.png)

Настроим динамическую маршрутизацию на роутерах A и B на основе протокола RIP второй версии для передачи информации между маршрутизаторами в сети.
![image](https://user-images.githubusercontent.com/58992611/231866937-864eab3b-5422-4994-948b-046c29bf8a58.png)

Теперь настроим телефонный сервис в автоматическом режиме. 
![image](https://user-images.githubusercontent.com/58992611/231866991-363f37b9-534a-48ca-a98c-a57ffb9fccc7.png)

Назначим диапазон портов.
![image](https://user-images.githubusercontent.com/58992611/231867033-bf6ec1a5-1fff-458d-9c3f-28962ddec462.png)

Создадим дополнительную конфигурацию. Для этого создаем первую логическую «телефонную» линию. Каждому телефону можно определить несколько таких логический линий со своими номерами. 
![image](https://user-images.githubusercontent.com/58992611/231867084-cc11b701-5192-4342-a63b-ce46d2d1c18b.png)

Произведем дополнительные настройки телефонии, позволяющие передавать звонки между удаленными сетями.
![image](https://user-images.githubusercontent.com/58992611/231867126-cec771ec-4542-4287-9968-ef4ded388419.png)

Был совершен успешный звонок из одной подсети в другую.
![image](https://user-images.githubusercontent.com/58992611/231867166-6b520c0a-dd0b-44d5-838e-5150c55e31cd.png)

Пинг между устройствами.
![image](https://user-images.githubusercontent.com/58992611/231867219-3851a2f4-e4af-44c4-862f-e9292acac39d.png)

**Вывод:** в ходе выполнения лабораторной работы был изучен алгоритм построения сети IP-телефонии между удаленными филиалами с помощью маршрутизаторов и коммутаторов.

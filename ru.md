## Model OSI and TCP/IP

## Концепция и базовые протоколы модели OSI

Open Systems Interconnection Basic Reference Model (OSI), 1978 г. – абстрактная сетевая модель для
коммуникаций и разработка сетевых протоколов. Представляет уровневый подход к сети.
Каждый уровень обслуживает свою часть процесса взаимодействия.
Благодаря такой структуре совместная работа сетевого оборудования и программного обеспечения
становится гораздо проще, прозрачнее и понятнее.

На сегодняшний день основным используемым стеком протоколов является TCP/IP, разработка которого не
было связано с моделью OSI и к тому же было осуществлено до ее принятия.
За все время существования модели OSI она не была реализована, и, по-видимому, не будет
реализована никогда. Сегодня используется только некоторое подмножество модели OSI.
Считается, что модель слишком сложна, а ее реализация займет слишком много времени.

Некоторые специалисты утверждают также, что история модели OSI представляет типичный пример.
неудачного и оторванного от жизни проекта.

| №   | Уровень       | Тип данных                                       | Функция                                     | Пример                                                      |
|-----|---------------|--------------------------------------------------|---------------------------------------------|-------------------------------------------------------------|
| 7   | Прикладной    | Сообщение                                        | Доступ к сетевым службам                    | HTTP, FTP, SMTP, DNS, SSH                                   |
| 6   | Представления | Данные                                           | Представление и шифрование данных           | ASCII, JPEG, GIF, SSL, TLS                                  |
| 5   | Сеансовый     | Данные                                           | Управление сетевым сеансом                  | NetBIOS, Sockets                                            |
| 4   | Транспортный  | Сегменты та датаграммы<br/>Segment<br/> Datagram | Прямое соединение между точками             | TCP, UDP                                                    |
| 3   | Сетевой       | Пакеты (Packets)                                 | Определение маршрута и логическая адресация | IPv4, IPv6, AppleTalk, Routers                              |
| 2   | Канальный     | Кадры (Frames)                                   | Физическая адресация (LLC, MAC)             | IEEE, Ethernet, DSL, Switches                               |
| 1   | Физический    | Биты (Bits)                                      | Сигналы, сетевая среда                      | USB, витая пара, оптический<br/> кабель, коаксиальный, хабы |

## Концепция и базовые протоколы стека TCP/IP

TCP/IP — сетевая модель передачи данных, представленных в цифровом виде.
Модель описывает способ передачи данных от источника информации к получателю.
В модели предполагается прохождение информации через четыре уровня, каждый из
которых описывается правилом (протоколом передачи). Наборы правил, решающих
задачу по передаче данных, составляют стек протоколов передачи данных, на
которых базируется Интернет.

Название TCP/IP происходит из двух важнейших протоколов семейства
*Transmission Control Protocol (TCP)* и *Internet Protocol (IP)*
Протоколы были первыми разработаны и описаны в данном стандарте.

| №   | Уровень                | Тип данных            | Функция                         | Пример                                                                             |
|-----|------------------------|-----------------------|---------------------------------|------------------------------------------------------------------------------------|
| 4   | Прикладной             | Сообщение             | Доступ к сетевым службам        | HTTP, FTP, SMTP, DNS, SSH, Telnet                                                  |
| 3   | Транспортный           | Сегменты и датаграммы | Прямое соединение между точками | TCP, UDP                                                                           |
| 2   | Уровень сети Интернет  | Пакет (Packets)       | Физическая адресация (LLC, MAC) | IPv4, IPv6, IPSec, AppleTalk                                                       |
| 1   | Уровень доступа к сети | Кадри (Frames)        | Сигналы, сетевая средае         | Ethernet, IEEE 802.11, USB, витая пара, оптический<br/> кабель, коаксиальный, хабы |

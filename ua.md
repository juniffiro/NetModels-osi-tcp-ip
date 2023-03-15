## Model OSI and TCP/IP

## Концепція та базові протоколи моделі OSI

Open Systems Interconnection Basic Reference Model (OSI), 1978 р. — абстрактна мережева модель для
комунікацій і розроблення мережевих протоколів. Представляє рівневий підхід до мережі.
Кожен рівень обслуговує свою частину процесу взаємодії.
Завдяки такій структурі спільна робота мережевого обладнання й програмного забезпечення
стає набагато простішою, прозорішою й зрозумілішою.

На сьогодні основним використовуваним стеком протоколів є TCP/IP, розроблення якого не
було пов'язане з моделлю OSI і до того ж було здійснено до її прийняття.
За увесь час існування моделі OSI вона не була реалізована, і, очевидно, не буде
реалізована ніколи. Сьогодні використовується тільки деяка підмножина моделі OSI.
Вважається, що модель занадто складна, а її реалізація займе забагато часу.

Окремі фахівці стверджують також, що історія моделі OSI являє типовий приклад
невдалого й відірваного від життя проєкту.

| №   | Рівень        | Тип даних                                       | Функція                                  | Приклади                                                 |
|-----|---------------|-------------------------------------------------|------------------------------------------|----------------------------------------------------------|
| 7   | Прикладний    | Повідомлення                                    | Доступ до мережевих служб                | HTTP, FTP, SMTP, DNS, SSH                                |
| 6   | Представлення | Дані                                            | Представлення та шифрування даних        | ASCII, JPEG, GIF, SSL, TLS                               |
| 5   | Сеансовий     | Дані                                            | Керування<br/> мережевим сеансом         | NetBIOS, Sockets                                         |
| 4   | Транспортний  | Сегменти та датаграми<br/>Segment<br/> Datagram | Пряме з'єднання між точками              | TCP, UDP                                                 |
| 3   | Мережевий     | Пакети (Packets)                                | Визначення маршруту та логічна адресація | IPv4, IPv6, AppleTalk, Routers                           |
| 2   | Канальний     | Кадри (Frames)                                  | Фізична адресація (LLC, MAC)             | IEEE, Ethernet, DSL, Switches                            |
| 1   | Фізичний      | Біти (Bits)                                     | Сигнали, мережеве середовище             | USB, вита пара, оптичний<br/> кабель, коаксиальний, хаби |

## Концепція та базові протоколи стека TCP/IP

TCP/IP – мережна модель передачі даних, представлених у цифровому вигляді.
Модель визначає спосіб передачі від джерела інформації до одержувачу.
У моделі передбачається проходження інформації через чотири рівні, кожен із
яких описується правилом (протоколом передачі). Набори правил, вирішальних
завдання передачі даних, становлять стек протоколів передачі, на
яких базується Интернет.

Назва TCP/IP походить з двох найважливіших протоколів сімейства
*Transmission Control Protocol (TCP)* та *Internet Protocol (IP)*
Протоколи першими розроблені та описані в цьому стандарті.

| №   | Рівень                   | Тип даних                                       | Функція                                  | Приклади                                                                        |
|-----|--------------------------|-------------------------------------------------|------------------------------------------|---------------------------------------------------------------------------------|
| 4   | Прикладний               | Повідомлення                                    | Доступ до мережевих служб                | HTTP, FTP, SMTP, DNS, SSH, Telnet                                               |
| 3   | Транспортний             | Сегменти та датаграми<br/>Segment<br/> Datagram | Пряме з'єднання між точками              | TCP, UDP                                                                        |
| 2   | Рівень мережі Internet   | Пакет (Packets)                                 | Визначення маршруту та логічна адресація | IPv4, IPv6, IPSec, AppleTalk                                                    |
| 1   | Рівень доступу до мережі | Кадри (Frames)                                  | Сигнали, мережеве середовище             | Ethernet, IEEE 802.11, USB, вита пара, оптичний<br/> кабель, коаксиальний, хаби |
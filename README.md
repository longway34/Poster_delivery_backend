# Проект автоматизации формирования заказов для поставщиков пользователей сервиса ["Poster"](https://joinposter.com/)

# Предполагаемое использование:

Для бухгалтеров/товароведов предприятий с большим количеством товаров и инградиентов, и значительным количеством поставщиков. 
Представляет возможность для каждого склада задавать расписание снятия остатков и автоматического формирования заказов для любого количества поставщиков исходя из заранее определенного минимального и/или желаемого количества продукта/инградиента на складе.

# [Серверная часть.](https://github.com/longway34/Poster_auto_suppliers_server)

Предназначена для:
1. Накопления, хранения и настроек проекта, таких как: 
* способы и адреса доставки заявок поставщикам; 
* минимальные и/или желательные остатки продуктов и инградиентов на каждом складе; 
* последние и/или согласованные с поставщиком объемы и цены заказываемых товаров и инградиентов.
* схема структуры БД представлена на [cheme_db.svg](https://raw.githubusercontent.com/longway34/Poster_auto_suppliers_server/master/cheme_db.svg)


![Схема БД](https://raw.githubusercontent.com/longway34/Poster_auto_suppliers_server/master/cheme_db.svg)


2. Формирование и доставку заявок согласно расписанию и/или по команде пользователя.
3. Формирование страниц администрирования, формироваия запросов к БД проекта и БД "Poster" посредством [API сервиса](https://dev.joinposter.com/docs/v3/start/index) и ручного формирования заказов.
4. Накопление и просмотр истории заказов поставщикам.

## Используемые программные продукты и службы:

* MySQL ver 14.14 Distrib 5.7.32, for Linux (x86_64)
* Node.js: 15.3.0, npm: 7.0.14
* Express version: 4.17.1 - http/https: сервер 

## Разработана в среде Visual Studio Code:
* Version: 1.51.1 (user setup)
* Date: 2020-11-10T23:34:32.027Z
* Electron: 9.3.3
* Chrome: 83.0.4103.122
* Node.js: 12.14.1
* V8: 8.3.110.13-electron.0
* OS: Windows_NT x64 10.0.18363

---

# [Клиентская часть.](https://github.com/longway34/Poster_auto_suppliers_client)

Обеспечивает пользователю возможность создание/изменение настроек расписания сбора остатков, формирования заказов (заявок), их отправку на заранее определенные адреса поставщиков, просмотр истории заказов (заявок).

![Настройка шаблонов](https://raw.githubusercontent.com/longway34/Poster_auto_suppliers_client/master/public/demo_images/Poster_Shablon.png "Настройка шаблонов")
Настройка шаблонов

![Настройка поставщиков](https://raw.githubusercontent.com/longway34/Poster_auto_suppliers_client/master/public/demo_images/Poster_Suppliers.png "Настройка поставщиков")
Настройка поставщиков

![Примеры заказов](https://raw.githubusercontent.com/longway34/Poster_auto_suppliers_client/master/public/demo_images/Poster_Supplies.png "Примеры заказов")
Примеры заказов

# Используемые программные продукты:
* Node.js: 15.3.0, npm 7.0.14
* React: 16.14.0
* Redux: 4.0.5
* react-router-dom: 5.2.0
* @material-ui/core: 4.11.1

# Разработана в среде Visual Studio Code 
* Version: 1.51.1 (user setup)
* Date: 2020-11-10T23:34:32.027Z
* Electron: 9.3.3
* Chrome: 83.0.4103.122
* Node.js: 12.14.1
* V8: 8.3.110.13-electron.0
* OS: Windows_NT x64 10.0.18363

---

На момент написания данного текста (28.11.2020) демо проект работает по [адресу http://longway34.ru/poster](http://longway34.ru/poster)

В репозитарии представлен демонстрационный вариант проекта, предполагающий следующие ограничения:

* Отстутствуют настройки доступа к реальным системам автоматизации учета "Poster".
* Отключены настройки UI (схемы, модели...)
* Проработка дизайна клиентской части проекта не проводилась. В ее реализации были использованы самые разнообразные элементы пакетов @material-ui. Целью было ознакомление автором достоинств и недостатков данного программного комплекса.
* Отключены настройки разделения доступа пользователей проекта
* Отключена подсистема развертывания для реальных условий эксплуатации.
* Способ доставки допускает только ручное формирование заявок и их рассылка по EMail. В системе кроме того предусмотрена ручная и автоматическая рассылка в Viber, Telegram.
* В репозитарии представлен минимально комментированный (рабочий) вариант не предусматривающий его распространения и  технической поддержки. Использование этого варианта допустимо дез всяких ограничений на Ва страх и риск.

По всем вопросам отвечу по адресу [E-Mail: longway34@gmail.com](mailto://longway34@gmail.com)

# Всем желаю удачи...
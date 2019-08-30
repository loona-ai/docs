---
layout: integration
title: Integration Documentation

search: true
home: false
---
# iiko
## Установка плагина
- Копируем папку LoonaPluginSettings в C:\Users\YourUserName\ProgramData\Roaming 

- Копируем папки LoonaPlugin и iikoWaiter5 в директорию iikoFront/Plugins (в нашем случае C:\Program Files\iiko\iikoRMS\Front.Net\Plugins)


- Запускаем iiko Front (помним что для данного метода нужна лицензии типа iikoTableService, iikoWaiter, iikoFrontPaymentPlugin)


- В iiko Front переходим в раздел “Дополнения” и выбираем “Loona settings”.

        login - Admin 

        password - Loona Admin

<img src="../images/iiko1.PNG" width="910" height="456" alt="Card Flip">
- Задаем настройки
        
        Api access token - по запросу
        Api base url - https://apidev.loona.ai
        Waiter request url - http://localhost
        Waiter port - 1234
<img src="../images/iiko2.png" width="512" height="288" alt="Card Flip">

- Открываем iiko Office
    - Переходим в раздел Дисконтная Система -> Скидки и Надбавки
    - Добавляем скидку
    - Обязательно пишем название - LoonaFixedSumDiscount
    - Тип скидки ставим Скидки и Надбавки
    - Нажимаем Далее
    
<img src="../images/iiko3.PNG" width="910" height="488" alt="Card Flip">

- Убираем галочку Можно назначить вручную, остальное по усмотрению ресторана

<img src="../images/iiko4.png" width="821" height="610" alt="Card Flip">

- Тип ставим “Фиксированная сумма” и обязательно устанавливаем галочку “Назначать сумму”

<img src="../images/iiko5.PNG" width="910" height="490" alt="Card Flip">

- Нажимаем Далее и заканчиваем установку скидки.


- Добавляем внешний вид оплаты. Переходим в раздел “Розничные продажи”  нажимаем на “Тип платы” и добавляем новую оплату. 
- Обязательно указываем: 

        наименование - Loona Payment
        Тип - Внешний тип оплаты
        Название в чеке - пишите что хотите
        Безналичный тип - Loona Payment 
- Сохраняем

<img src="../images/iiko6.png" width="512" height="266" alt="Card Flip">

- Устанавливаем мобильное приложение iikoWaiter5

- Перезагружаем iiko front

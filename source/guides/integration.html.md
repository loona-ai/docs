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

   > Login - Admin   
   Password - Loona Admin

<img src="../images/iiko1.PNG" width="910" height="456">
- Задаем настройки
        
 >  Api access token - по запросу  
    Api base url - https://apidev.loona.ai  
    Waiter request url - http://localhost  
    Waiter port - 1234
>
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

    >   Наименование - Loona Payment  
        Тип - Внешний тип оплаты  
        Название в чеке - пишите что хотите  
        Безналичный тип - Loona Payment
- Сохраняем

<img src="../images/iiko6.png" width="512" height="266" alt="Card Flip">

- Устанавливаем мобильное приложение iikoWaiter5

- Перезагружаем iiko front

## Настройки в кабинете

# r_keeper

## Установка плагина

*В течении использования плагина, нужно выключить Windows Firewall или открыть доступ для порта плагина (port 1234)

-	Скачайте папку Loona R-keeper

-	Откройте папку Loona R-keeper

 <img src="../images/rk1.png" width="747" height="190">

-	Скопируйте «Extdll.dll» и «Extdll.ini» в папку UCS/FARCARDS
 
 <img src="../images/rk2.png" width="738" height="669">

-	Откройте файл «FARCARDS.INI» в текстовом редакторе

-	В поле DLL впишите «ExtDll.dll» и сохраните изменения
 
 <img src="../images/rk3.png" width="757" height="420">

-	Запустите  «Farcards.exe – install»

-	Откройте папку где содержится R-keeper и запустите R-keeper «Manager»
 
 <img src="../images/rk4.png" width="746" height="189">

-	Откройте систему r_keeper и зайдите в неё


-	Пройдите в меню в раздел «Деньги» и откройте «Скидки и Наценки»
 
 <img src="../images/rk5.png" width="1167" height="581">

-	Откроется окно управления скидок и наценок, наведите мышь на поле «All» и с помощью правой кнопки мышки создайте новый тип скидок
 
 <img src="../images/rk6.png" width="1218" height="424">

-	Откроются «Свойства», в них введите Название своей скидки и поменяйте статус на Активный
 
 <img src="../images/rk7.png" width="696" height="260">

-	Пройдите в окно «Скидки/Нацинки» вашей новой скидки и создайте новую скидку (Нажмите правой кнопки мышки на свободое поле, из возникших опций выберите «Новая скидка»)
 
 <img src="../images/rk8.png" width="1225" height="379">

-	Введите название вашей скидки, пока что не меняйте статус на активный
 
 <img src="../images/rk9.png" width="1219" height="702">

-	Откройте детализацию вашей скидки двойным кликом на иконку
 
 <img src="../images/rk10.png" width="414" height="150">

-	Создайте новую детализацию (Нажмите правой кнопки мышки на свободое поле, из возникших опций выберите «Новая детализация»)
 
 <img src="../images/rk11.png" width="345" height="347">

-	Откройте поле настроек детализации, и поменяйте процент скидки на 100.00
 
 <img src="../images/rk12.png" width="1213" height="400">

-	Сохраните изменения 

<img src="../images/rk13.png" width="1494" height="700">

-	Пройдите обранто в «Свойства» вашей скидки и поменяйте статус на активный «Active»

 <img src="../images/rk14.png" width="1214" height="627">

-	Сохраните изменения, но еще не закрывайте окно «Скидки и Надбавки»

-	Откройте папку Loona R-keeper

-	Скопируйте папку Loona в папку где хратится r_keeper и FARCARDS

 <img src="../images/rk15.png" width="750" height="425">

-	Откройте скопированую папку Loona, и запустите из нее файл «ServiceInstaller.exe» как администратор

 <img src="../images/rk16.png" width="741" height="412">

-	Сервис будет установлен, после установки зайдите в Windows  Services (Сервисы), найдите Loona r-keeper plugin и убедитесь что «Startup Type» стоит автоматичекий (Automatic)

 <img src="../images/rk17.png" width="1265" height="872">

-	Не закрывайте окно сервисов

-	Затем откройте ваш браузер

-	Введите адрес плагина в браузере, адрес: «localhost:1234/settings»

-	Откроется поле настроек плагина. Введите необходимые параметры для настройки скидки и сохраните параметры. Код вашей скидки вам доступен в свойствах скидки в r_keeper manager.

 <img src="../images/rk18.png" width="1008" height="637">

> Для получения Идентификационного номера сканера и URL кабинета обратитесь к документации кабинета Loona  

> При изменениях порта на «XXXX», адрес плагина меняется на localhost:XXXX/settings (но нет необходимости менять порт)  

<img src="../images/rk19.png" width="1219" height="714">

-	Сохраните изменения параметров плагина

-	Вернитесь в «Сервисы», выделите сервис Loona r-keeper plugin, обновите сервис (сервис должен выключится после обновления), затем запустите сервис

 <img src="../images/rk20.png" width="1259" height="868">



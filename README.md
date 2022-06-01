# **Проведение нагрузочного тестирования WEB**

**Ссылка на задания/требования:** https://github.com/netology-code/loadqa-homeworks/blob/main/3.Load%20web/homework_lecture3.md

## **Тестирования действий пользователя на сайте блога: https://qamidhl.herokuapp.com/**

**Cценарий тестирования действий пользователя на сайте блога: https://qamidhl.herokuapp.com/**

1. Открыть блог https://qamidhl.herokuapp.com/
2. Авторизоваться под пользователем: qamidl1/ ‘qamidl1.netology.ru’
3. Открыть пост https://qamidhl.herokuapp.com/?p=1
4. Добавить комментарий заполнив поле Comment

**Записанный сценарий в формате jmx:** https://github.com/Dmitruzd21/JMeterAndBlazeMeter/blob/master/QAMIDHL_folder/QAMIDHL.jmx

**Cкриншот о выполнении сценария в JMeter с помощью `View Results Tree`**

![JMeter1](/QAMIDHL_folder/JMeter/QAMIDHL1.jmx.png)

**Cкриншоты отчетов JMeter о проведенном тестировании**

![JMeter2](/QAMIDHL_folder/JMeter/QAMIDHLResponceCodesPerSecond.png)

![JMeter3](/QAMIDHL_folder/JMeter/QAMIDHLSummaryReport.png)

**Cкриншоты получившейся нагрузки в системе BlazeMeter**

![BlazeMeter1](/QAMIDHL_folder/BlazeMeter/BM1.png)

![BlazeMeter2](/QAMIDHL_folder/BlazeMeter/BM2.png)

![BlazeMeter3](/QAMIDHL_folder/BlazeMeter/BM3.png)

![BlazeMeter4](/QAMIDHL_folder/BlazeMeter/BM4.png)

![BlazeMeter5](/QAMIDHL_folder/BlazeMeter/BM5.png)

![BlazeMeter6](/QAMIDHL_folder/BlazeMeter/BM6.png)

![BlazeMeter7](/QAMIDHL_folder/BlazeMeter/BM7.png)

![BlazeMeter8](/QAMIDHL_folder/BlazeMeter/BM8.png)

![BlazeMeter9](/QAMIDHL_folder/BlazeMeter/BM9.png)

![BlazeMeter10](/QAMIDHL_folder/BlazeMeter/BM10.png)

![BlazeMeter11](/QAMIDHL_folder/BlazeMeter/BM11.png)

## **Тестирование покупки билета в кинотеатре и получение QR кода**

**Cценарий тестирования покупки билета и получение QR кода**

1. Открыть страницу в Chrome по url - http://localhost:8000/client/index.php

Ожидание: 3000 мс

2. Выбрать следующий день

Ожидание: 3000 мс

3. Выбрать Фильм 3 - Зал 1 - Сеанс на 11:10

Ожидание: 3000 мс

4. Выбрать место (например, ряд 1, кресло 1)

Ожидание: 3000 мс

5. Клик по кнопке "Забронировать"

Ожидание: 3000 мс

6. Клик по кнопке "Получить код бронирования"

**Записанный сценарий в формате jmx:** https://github.com/Dmitruzd21/JMeterAndBlazeMeter/blob/master/Cinema_folder/Cinema.jmx_changes.png

**Примечание:** Для воспроизведения сценария необходимо изменить параментр seanceTimeStamp во втором запросе (Select Day). Этот параметр изменяется каждый день.

**Cкриншот о выполнении сценария в JMeter с помощью `View Results Tree`**

![ViewResultsTree](/Cinema_folder/JMeter/Cinema_ViewTree.png)

**Cкриншоты отчетов JMeter о проведенном тестировании**

![JMeter1](/Cinema_folder/JMeter/JMeter1.png)

![JMeter2](/Cinema_folder/JMeter/JMeter2.png)

![JMeter3](/Cinema_folder/JMeter/JMeter3.png)

![JMeter4](/Cinema_folder/JMeter/JMeter4.png)

![JMeter5](/Cinema_folder/JMeter/JMeter5.png)

![JMeter6](/Cinema_folder/JMeter/JMeter6.png)

![JMeter7](/Cinema_folder/JMeter/JMeter7.png)

**Cкриншоты полученных результатов из системы монитронига (InfluxDB)**

![](/Cinema_folder/InfluxDB/JMeter_InfluxDB1.png)

![](/Cinema_folder/InfluxDB/JMeter_InfluxDB2.png)

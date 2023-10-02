# Power BI practic projects

## 01 Автодиллер продажи по регионам
![Дашборд 01](https://github.com/ArtemFilosofGB/PowerBIpractics/blob/main/01_Autodealler/01.JPG)
## 02 Выгрузка cbrf
## 03 Тестовое заданеи Сфера
![Дашборд 03](https://github.com/ArtemFilosofGB/PowerBIpractics/blob/main/03_Cфера%20тестовое%20задание/Тестовой%20задание%201%20230923.JPG)
## 04 ТЗ
## 05 Аско
![Дашборд 05](05_Asko_task/DashboardAsko.PNG)


## Полезные пямятки
### Создание календаря
    * Dates  =
    GENERATE (
    CALENDAR ( DATE ( 2017, 1, 1 ), DATE ( 2017, 12, 31 ) ),
    VAR currentDay = [Date]
    VAR day = DAY( currentDay )
    VAR month =  MONTH ( currentDay )
    VAR year =  YEAR ( currentDay )
    RETURN   ROW (
    "day", day,
    "month", month,
    "year", year )
    )

  https://powerbi.tips/2017/11/creating-a-dax-calendar/

  ## Редактирование таблицы календаря

    * Calendar = CALENDAR(MIN('Таблица 3 (СПР_даты_заказа)'[Дата].[Date]), MAX('Таблица 3 (СПР_даты_заказа)'[Дата].[Date]))
    * MobthYear = FORMAT('Calendar'[Date],"mmm'yy")# PowerBIpractics


[def]: https://github.com/ArtemFilosofGB/PowerBIpractics/blob/main/03_Cфера%20тестовое%20задание/Тестовой%20задание%201%20230923.JPG
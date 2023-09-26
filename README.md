# 01 

# Создание календаря
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

  # Редактирование таблицы календаря

    * Calendar = CALENDAR(MIN('Таблица 3 (СПР_даты_заказа)'[Дата].[Date]), MAX('Таблица 3 (СПР_даты_заказа)'[Дата].[Date]))
    * MobthYear = FORMAT('Calendar'[Date],"mmm'yy")# PowerBIpractics

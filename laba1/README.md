# Получение сведений о системе

## Цель работы

Получить сведения об используемой системе

## Исходные данные

1. Ноутбук Lenovo

2. Windows



## План

1. Ввод команд в эмулятор терминала

2. Анализ данных

## Ход работы


1. Затем получим сведения о версии ядра:

winver


В результате выполнения данной команды была получена версия ядра - 22H2(сборка ОС 19045.2728)

2. Далее можно получить сведения о процессоре:

```
#1я команда
Get-WmiObject win32_Processor
Caption           : Intel64 Family 6 Model 60 Stepping 3
DeviceID          : CPU0
Manufacturer      : GenuineIntel
MaxClockSpeed     : 2401
Name              : Intel(R) Core(TM) i7-4700MQ CPU @ 2.40GHz
SocketDesignation : U3E1


3. Далее получим последние 30 строк логов системы:

```
Get-EventLog -LogName 'system' -Newest 30

     Index Time          EntryType   Source                 InstanceID Message
   ----- ----          ---------   ------                 ---------- -------
   69532 апр 07 22:53  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69531 апр 07 22:53  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69530 апр 07 22:52  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69529 апр 07 22:52  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69528 апр 07 22:49  Information Microsoft-Windows...           16 Не найдено описание для события с кодом '16' в исто...
   69527 апр 07 22:45  Information Microsoft-Windows...           16 Не найдено описание для события с кодом '16' в исто...
   69526 апр 07 22:45  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69525 апр 07 22:38  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69524 апр 07 22:35  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69523 апр 07 22:35  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69522 апр 07 22:34  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69521 апр 07 22:34  Information Microsoft-Windows...           16 Не найдено описание для события с кодом '16' в исто...
   69520 апр 07 22:11  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69519 апр 07 22:03  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69518 апр 07 20:40  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69517 апр 07 20:40  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69516 апр 07 20:39  Information Service Control M...   1073748864 Тип запуска службы "Фоновая интеллектуальная служба...
   69515 апр 07 20:35  Information Service Control M...   1073748864 Тип запуска службы "Фоновая интеллектуальная служба...
   69514 апр 07 20:17  Information Service Control M...   1073748864 Тип запуска службы "Фоновая интеллектуальная служба...
   69513 апр 07 18:46  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69512 апр 07 17:56  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69511 апр 07 17:56  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69510 апр 07 17:56  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69509 апр 07 17:55  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69508 апр 07 17:55  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69507 апр 07 17:54  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69506 апр 07 17:54  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69505 апр 07 17:54  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69504 апр 07 17:54  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...
   69503 апр 07 17:54  Warning     DCOM                        10016 Не найдено описание для события с кодом '10016' в и...


## Оценка результата

В результате лабораторной работы была получена базовая информация об используемой системе.

## Вывод

Таким образом. мы научились, используя команды Windows, получать сведения о системе.



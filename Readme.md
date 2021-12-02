# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

27.11.2021 - 28.11.2021 было проведено функциональное тестирование методом черного ящика приложения Credit Card Number Validator.

На тестирование затрачено: 1 час

В результате тестирования выявлены следующие дефекты:
* При использовании карт American express выходит ошибка.
#### Скриншот:
![American express fatal 1](https://user-images.githubusercontent.com/93321774/143690729-4096c8d6-879c-4e45-ad6b-a730fe4eb18a.png)
* При использовании карт Visa с номером карты выше 16 цифр выходит ошибка.
#### Скриншот:
![Visa длинный номер](https://user-images.githubusercontent.com/93321774/143690733-9ea66761-23fe-458c-a57f-30521cb08bfc.png)
* При использовании карт JBL с номером карты выше 16 цифр выходит ошибка.
#### Скриншот:
![JCB длинный](https://user-images.githubusercontent.com/93321774/143690731-7cbbc9ff-ea43-4c46-8662-8d3d242bec5c.png)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* Отчет о тестировании


В качестве тестовых данных использовались данные с сайта https://www.freeformatter.com/credit-card-number-generator-validator.html:

* При использовании данных карт Visa из 16 цифр программа исполнялась штатно
* При использовании данных карт MasterCard из 16 цифр программа исполнялась штатно
* При использовании данных карт JBL из 16 цифр программа исполнялась штатно
* При использовании данных карт Diners Club - North America из 16 цифр программа исполнялась штатно
* При использовании данных карт Maestro из 16 цифр программа исполнялась штатно
* При использовании данных карт Visa Electron из 16 цифр программа исполнялась штатно

Тестирование производилось в следующем окружении:
* Windows 10 64-разрядная
* Java 11.0.13+8 (х64)
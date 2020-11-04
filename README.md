# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

3/11/2020 23:14 -3/11/2020 было проведено функциональное тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 1

В результате тестирования выявлены следующие дефекты:
* [Ошибочная валидация Diners Club - Carte Blanche](https://github.com/dekotamin/credircard/issues/1) 
* [Ошибочная валидация American Express (Amex)](https://github.com/dekotamin/credircard/issues/2)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* приложение Credit Card Number Validator
* https://www.freeformatter.com/credit-card-number-generator-validator.html#fakeNumbers

В качестве тестовых данных использовались данные https://www.freeformatter.com/credit-card-number-generator-validator.html#fakeNumbers:

    VISA:
    4916896856049735          Result Ok
    4532361628782752          Result Ok
    4539411355585107687       Result Fail 
    
    MasterCard: 
    5583686106641004          Result Ok 
    5308576596676806          Result Ok
    5276877189990127          Result Ok 
    
    American Express (AMEX):
    370995389368823           Result Ok
    379185551859681           Result Ok
    379434926921903           Result Ok
    
    Discover:
    6011427519936081          Result Ok
    6011101693309890          Result Ok
    6011187171959921961       Result Fail
    
    JCB:
    3541194339132673          Result Ok
    3538251220616084          Result Ok
    3537090207210651253       Result Fail
    
    Diners Club - North America:
    5547196615345837          Result Ok
    5517875442448551          Result Ok
    5411306243179846          Result Ok
    
    Diners Club - Carte Blanche:
    30165866950277            Result Ok
    30262904419348            Result Ok
    30498071624001            Result Ok

Тестирование производилось в следующем окружении:
* Ubuntu 20.04 amd 64bit
* Java 11.0.9
* Intellij IDEA
* Credit Card Number Validator


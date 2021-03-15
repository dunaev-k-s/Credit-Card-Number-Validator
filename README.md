# Отчёт о тестировании Credit Card Number Validator
## Краткое описание

**11.03.21 - 11.03.21** было проведено Smoke-тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 0.5 часа

В результате тестирования выявлены следующие дефекты:
* [Валидный номер карты Visa не прошел валидацию в Credit Card Number Validator](https://github.com/dunaev-k-s/Credit-Card-Number-Validator/issues/1)
* [Валидный номер карты Discover не прошел валидацию в Credit Card Number Validator](https://github.com/dunaev-k-s/Credit-Card-Number-Validator/issues/2)

## Описание процесса тестирования

В качестве тестовых данных использовались данные из [Credit Card Number Generator & Validator](https://www.freeformatter.com/credit-card-number-generator-validator.html#fakeNumbers)
* Ожидаемый результат **OK**: *VISA* 
  
```4532154391414442 4539341767324221 4916978431117743193 4929790288508798296 6011885403846354949```
* Ожидаемый результат **FAIL**: *VISA* 
  
```6532154391414442 6539341767324221 6916978431117743193```
* Ожидаемый результат **OK**: *MasterCard* 

```4532154391414442 4539341767324221 4916978431117743193```
  
* Ожидаемый результат **FAIL**: *MasterCard* 

```3532154391414442 3539341767324221 3916978431117743193```

Тестирование производилось в следующем окружении:
* Windows 10 20H2 x64
* OpenJDK 11.0.2
* IntelliJ IDEA 2020.3.2

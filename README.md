## Отчёт о тестировании приложения Money Transfer

При вводе в приложение заданных значений программа выдает некорректный результат. Проверка кода показала, что переменная total имеет неверный тип данных. Итоговое количество символов переменной total превысило допустимое значение для типа данных int. Также при используемом типе переменных невозможно отобразить дробную часть - сумму с  копейками.
 
## Описание тестов

Проводилось позитивное функциональное тестирование. Проводилось тестирование модуля программы Money Transfer, ответственного за отображение баланса счета клиента после транзакций.

## Результаты

1. При присвоении переменной total значения, соответствующего типу данных int, программа возвращает корректный результат. В противном случае - возвращается результат с ошибкой, а имеено минусовым балансом в итоге . Суммы с дробной частью - с копейками,  невозможно ввести в переменные с типом int.
2. [Неверный тип данных для переменных](https://github.com/Gnucheva/Money-Transfer/issues/1)

## Общие рекомендации

Необходимо задать переменным bill, transfer, total тип long double 
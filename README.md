# Отчёт о тестировании приложения **"MoneyTransfer"**

## Краткое описание

При функциональном тестировании приложения MoneyTransfer, была обнаружена **ошибка**. Консоль отображает отрицательное значение 
переменной ```currentBalance``` (которая содержит в себе информацию 
об итоговом балансе клиента) в тех случаях, когда её значение превышает **2_147_483_647**

## Описание тестов

Было проведено позитивное функциональное тестирование.

Тестировалась функция сложения текущих денежных средств с поступающими при поплнении баланса;

## Результаты

1. 50% неуспешных тестов

2. Ссылка на баг-репорт: https://github.com/camenzindmp/MoneyTransferTask/issues

## Общие рекомендации

Использовать примитивный целочисленный тип данных ```long``` **для VIP-аккаунтов**;

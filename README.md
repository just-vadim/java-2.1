# Отчёт о тестировании transfer

## Краткое описание

04.08.2020 - было проведено функцональное тестирование приложения transfer.

На тестирование затрачено: 20m

В результате тестирования выявлены следующие дефекты:
* [Некорректный результат работы программы transfer #1](https://github.com/just-vadim/java-2.1/issues/1)

## Описание процесса тестирования

Входные данные:
* текущий баланс счёта клиента - переменная типа int, значение - 2_000_000_000 (два миллиарда рублей)
* сумма перевода - переменная типа int, значение - 500_000_000 (пятьсот миллионов рублей)
* переменная для хранения итогового значения - тип int

Код программы:
```java
public class transfer {
    public static void main(String[] args) {
        int balance = 2000000000;
        int transfer = 500000000;
        int total = balance + transfer;
        System.out.println(total);
    }
}
```

Тестирование производилось в следующем окружении:
* ОС: Windows 10 Pro 1909 18363.959 x64
* Java: openjdk version "11.0.8" 2020-07-14;
OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.8+10);
OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.8+10, mixed mode)
* IDE: IntelliJ IDEA Community Edition 2020.2

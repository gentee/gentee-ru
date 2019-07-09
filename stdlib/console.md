---
nav: tocru
---

# Консоль

Здесь описаны функции для работы с консолью.

* [Print\( anytype par... \) int](console.md#printanytype-par-int)
* [Println\( anytype par... \) int](console.md#printlnanytype-par-int)
* [ReadString\( str text \) str](console.md#readstringstr-text-str)

## Операторы

| Оператор | Результат | Описание |
| :--- | :--- | :--- |
| **\|\|** str | int | Этот унарный оператор выводит строку в стандартный вывод, но перед этим он удаляет крайние пробельные символы в каждой строке. Возвращает количество записанных байтов. |

```text
run {
   ||`One
      Two
      Three
      `
}
/* It prints
One
Two
Three
*/
```

## Функции

### Print\(anytype par...\) int

Функция _Print_ форматирует по умолчанию все переданные операнды любых типов и выводит их в стандартный вывод. Пробелы являются разделителями при выводе параметров, если ни один из соседних параметров не является строкой. Функция _Print_ возвращает количество записанных байтов.

### Println\(anytype par...\) int

Функция _Println_ форматирует по умолчанию все переданные операнды любых типов и выводит их в стандартный вывод. Также, она записывает в конце символ перевода строки. Пробелы всегда являются разделителями при выводе параметров. Функция _Println_ возвращает количество записанных байтов.

### ReadString\(str text\) str

Функция _ReadString_ читает данные из стандартного ввода до получения символа '\n' \(нажатие Enter\). Она возвращает строку содержащую введенные данные. Если параметр _text_ не пустой, то функция выведет этот текст перед чтением данных.

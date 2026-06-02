# Работа со строками в Java — варианты для практики

Здесь два простых кода на Java, которые помогают мне тренировать **работу со строками**.

Первый — выводит каждый символ строки `"Hello"` по одному.  
Второй — выводит символы строки `"Java"` в обратном порядке.  

## Вариант 1: выводим символы строки "Hello"

**Что делает:**  
Проходит по строке `"Hello"` от первого символа до последнего и выводит каждый символ с новой строки.

**Код:**

```java
    public static void main(String[] args) {
        System.out.println(loop());
    }

    public static String loop() {
        String result = "";
        String str = "Hello";
        for (int i = 0; i < str.length(); i++) {
            result += str.charAt(i) + "\n";
        }
        return result;
    }
```

#### Пример вывода в консоли

H  
e  
l  
l  
o  

---

## Вариант 1: выводим символы строки "Java" в обратном порядке

**Что делает:**

Проходит по строке "Java" с конца в начало и выводит каждый символ с новой строки.

**Код:**

```java
    public static void main(String[] args) {
        System.out.println(loop());
    }

    public static String loop() {
        String result = "";
        String str = "Java";
        for (int i = str.length() - 1; i >= 0; i--) {
            result += str.charAt(i) + "\n";
        }
        return result;
    }
```

#### Пример вывода в консоли

a  
v  
a  
J  

---

## Мои заметки для запоминания
- `str.length()` — длина строки
- `str.charAt(i)` — символ по индексу `i`
- `i <= str.length() - 1` — последний индекс строки
- Цикл от конца к началу: `i = str.length() - 1; i >= 0; i--`

---


⭐ Этот файл — моя шпаргалка по циклам и работе со строками.

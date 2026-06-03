# Вариант 1: charAt
**Что делает:**  
Проходит по строке "Hello" от первого символа до последнего и выводит каждый символ с новой строки.

**Код:**
```java
    public static void main(String[] args) {
        String str = "Hello";
        System.out.println(loop(str));
    }

    public static String loop(String str) {
        String result = "";
        for (int i = 0; i < str.length(); i++) {
            result += str.charAt(i) + "\n";
        }
        return result;
    }
```
#### Пример вывода в консоли:

H  
e  
l  
l  
o  

---

# Вариант 2: количество символов в строке

**Что делает:**  
Подсчитывает, сколько раз буква "l" встречается в строке "Hello world".

**Код:**
```java
    public static void main(String[] args) {
        String str = "Hello world";
        int count = 0;

        for (int i = 0; i < str.length(); i++) {
            if (str.charAt(i) == 'l') count++;
        }
        System.out.println("Количество букв l: " + count);
    }
```
#### Пример вывода в консоли:
Количество букв l: 3

---

# Вариант 3: символ + его индекс

**Что делает:**  
Выводит каждый символ строки "Hello" вместе с его индексом.

**Код:**

```java
    public static void main(String[] args) {
        String str = "Hello";

        for (int i = 0; i < str.length(); i++) {
            System.out.println(str.charAt(i) + ": " + i);
        }
    }
```
#### Пример вывода в консоли:
H: 0  
e: 1  
l: 2  
l: 3  
o: 4  

---

### Мои заметки:
- `charAt(i)` — символ на позиции `i`
- `charAt(i)` — берёт символ по индексу `i`
- `charAt(i) == 'l'` — сравниваем символ с буквой `l`
- Счётчик `count++` увеличивается при каждом совпадении
- В строке `"Hello world"` буква `l` встречается `3` раза
- Полезно для понимания, как нумеруются символы в строке
- Индексы начинаются с `0`, а не с `1`

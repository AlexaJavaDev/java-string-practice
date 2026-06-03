# Вариант 1
**Что делает:**  
Находит индекс первого вхождения буквы "o" в строке "Hello world".

**Код:**
```java
    public static void main(String[] args) {
        String str = "Hello world";
        int a = str.indexOf("o");
        System.out.println(loop(a));
    }

    public static int loop(int a) {
        return a;
    }
```
Или сделать попроще, без отдельного метода:

```java
public class IndexOfSimpleExample {
    public static void main(String[] args) {
        String str = "Hello world";
        System.out.println(str.indexOf("o"));
    }
```

#### Пример вывода в консоли:
4

---

### Мои заметки:
- `indexOf(символ)` — возвращает индекс первого вхождения
- Индексы начинаются с 0: 'H' = 0, 'e' = 1, 'l' = 2, 'l' = 3, 'o' = 4
- Если символ не найден, вернёт -1

# Вариант 2: lastIndexOf

**Что делает:**  
Находит индекс последнего вхождения буквы "o" в строке "Hello world".

**Код:**

```java
    public static void main(String[] args) {
        String str = "Hello world";
        int a = str.lastIndexOf("o");
        System.out.println(loop(a));
    }

    public static int loop(int a) {
        return a;
    }
```

Или проще:

```java
    public static void main(String[] args) {
        String str = "Hello world";
        System.out.println(str.lastIndexOf("o"));
    }
```
#### Пример вывода в консоли:
7

---

### Мои заметки:
- `lastIndexOf(символ)` — ищет с конца строки
- Возвращает индекс последнего вхождения
- Если символ один, результат совпадёт с `indexOf()`

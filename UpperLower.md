# 1. toUpperCase

**Что делает:**  
Переводит строку "Hello world" в верхний регистр (заглавные буквы).

**Код:**
```java
    public static void main(String[] args) {
        String str1 = "Hello world";
        System.out.println(loop(str1));
    }

    public static String loop(String str1) {
        return str1.toUpperCase();
    }
```
#### Пример вывода в консоли:

HELLO WORLD

---

### Мои заметки:
- `toUpperCase()` — все буквы становятся заглавными
- Русские буквы тоже работают: "привет" → "ПРИВЕТ"
- Оригинальная строка не меняется (строки в Java неизменяемы)

---

# 2. toLowerCase

**Что делает:**  

Переводит строку "HELLO WORLD" в нижний регистр (строчные буквы).

**Код:**
```java
    public static void main(String[] args) {
        String str1 = "HELLO WORLD";
        System.out.println(loop(str1));
    }

    public static String loop(String str1) {
        return str1.toLowerCase();
    }
```
#### Пример вывода в консоли:

hello world

---

### Мои заметки:
- `toLowerCase()` — все буквы становятся строчными
- Полезно для сравнения строк без учёта регистра
- Оригинальная строка остаётся неизменной

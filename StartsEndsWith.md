# 1. StartsWith
**Что делает:**  
Проверяет, начинается ли строка "Hello world" с "Hello".

**Код:**  
```java
    public static void main(String[] args) {
        String str1 = "Hello world";
        System.out.println(loop(str1));
    }

    public static String loop(String str1) {
        return str1.startsWith("Hello") ? "true" : "false";
    }
```
#### Пример вывода в консоли:  
true

---

### Мои заметки:
- `startsWith("строка")` — проверяет начало строки
- Возвращает `true` или `false`
- Чувствителен к регистру

---

# EndsWith
**Что делает:**  
Проверяет, заканчивается ли строка "Hello world" на "world".

**Код:**

```java
    public static void main(String[] args) {
        String str1 = "Hello world";
        System.out.println(loop(str1));
    }

    public static String loop(String str1) {
        return str1.endsWith("world") ? "true" : "false";
    }
```

#### Пример вывода в консоли:
true

---

### Мои заметки:
- `endsWith("строка")` — проверяет конец строки
- Возвращает `true` или `false`
- Чувствителен к регистру

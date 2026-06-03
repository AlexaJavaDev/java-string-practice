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

# 2. EndsWith
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

# 3. StartsAndEnds

**Что делает:**  
Проверяет, начинается ли строка "Hello world" с "Hello" и заканчивается ли на "world".
Возвращает true, если оба условия выполняются.

**Код:**
```java
    public static void main(String[] args) {
        String str = "Hello world";
        System.out.println(str.startsWith("Hello") && str.endsWith("world"));
    }
```
#### Пример вывода в консоли:
true

---

### Мои заметки:
- `endsWith("строка")` — проверяет конец строки
- `startsWith("строка")` — проверяет начало строки
- Возвращает `true` или `false`
- Чувствителен к регистру
- `&&` означает «и» (оба условия должны быть `true`)
- Можно комбинировать любые проверки через `&&` (и) или `||` (или)
- Строка "Hello world" начинается с "Hello" и заканчивается на "world" → true

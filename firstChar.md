**Что делает:**  
Выводит первый символ строки "Hello".

**Код:**
```java
    public static void main(String[] args) {
        String str = "Hello";
        System.out.println(loop(str));
    }

    public static String loop(String str) {
        return "Первый символ: " + str.charAt(0);
    }
```
#### Пример вывода в консоли:

Первый символ: H

---

### Мои заметки:  
- Первый символ всегда под индексом 0
- Если строка пустая, charAt(0) вызовет ошибку

**Что делает:**  
Складывает длины двух строк "Hello" и "World".

**Код:**
```java
    public static void main(String[] args) {
        String str1 = "Hello";
        String str2 = "World";
        System.out.println(loop(str1, str2));
    }

    public static String loop(String str1, String str2) {
        int a = str1.length();
        int b = str2.length();
        int c = a + b;
        return "Длина строки: " + c;
    }
```

#### Пример вывода в консоли:

Длина строки: 10

---
### Мои заметки:
- `str1.length() + str2.length()` = общая длина
- Можно складывать прямо в `return`, без отдельных переменных

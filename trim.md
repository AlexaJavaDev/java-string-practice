**Что делает:**  
Убирает пробелы в начале и в конце строки " Hello world ".

**Код:**
```java
    public static void main(String[] args) {
        String str1 = " Hello world ";
        System.out.println(loop(str1));
    }

    public static String loop(String str1) {
        return str1.trim();
    }
```
#### Пример вывода в консоли:

|Hello world|  
где `| |` границы - пробелы убраны

---

### Мои заметки:
- `trim()` убирает только пробелы в начале и конце
- Пробелы между словами остаются
- Убирает `' '` (пробел), `\t` (табуляцию), `\n` (перенос строки)

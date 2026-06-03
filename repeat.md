**Что делает:**  
Повторяет строку "Java" 3 раза подряд.

**Код:**
```java
    public static void main(String[] args) {
        String str1 = "Java";
        System.out.println(loop(str1));
    }

    public static String loop(String str1) {
        return str1.repeat(3);
    }
```
#### Пример вывода в консоли:

JavaJavaJava

---

### Мои заметки:

- `repeat(N)` — повторяет строку `N` раз без пробелов
- Если `N = 0`, вернёт пустую строку
- Если `N = 1`, вернёт ту же строку

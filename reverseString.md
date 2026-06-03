**Что делает:**  
Выводит символы строки "Java" в обратном порядке (с конца в начало).

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
#### Пример вывода в консоли:
a
v
a
J

---

### Мои заметки:
- Цикл идёт от последнего индекса `(length() - 1)` до первого `(0)`
- `i--` уменьшает счётчик, чтобы двигаться назад
- Так можно развернуть любую строку

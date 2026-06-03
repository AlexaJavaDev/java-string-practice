**Что делает:**  
Проверяет, содержит ли строка "Hello world and Java" слово "and".

**Код:**

```java
    public static void main(String[] args) {
        String str = "Hello world and Java";
        System.out.println(loop(str));
    }

    public static String loop(String str) {
        return str.contains("and") ? "true" : "false";
    }
```
#### Пример вывода в консоли:

true

---

### Мои заметки:
- `contains("слово")` — проверяет, есть ли слово внутри строки
- Возвращает `true`, или `false` - если не содержит
- Чувствителен к регистру: "And" не найдёт

**Что делает:**  
Выводит последний символ строки "Hello".

**Код:**  
```java
    public static void main(String[] args) {
        String str = "Hello";
        System.out.println(loop(str));
    }

    public static String loop(String str) {
        return "Последний символ: " + str.charAt(str.length() - 1);
    }
```
#### Пример вывода в консоли

Последний символ: o

---

### Мои заметки:
- Последний индекс = `str.length() - 1`
- Формула работает для любой строки
- Если строка пустая, будет ошибка

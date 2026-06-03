**Что делает:**  
Заменяет все буквы "o" на цифру "0" в строке "Hello world".

**Код:**
```java
    public static void main(String[] args) {
        String str1 = "Hello world";
        System.out.println(loop(str1));
    }

    public static String loop(String str1) {
        return str1.replace("o", "0");
    }
```

#### Пример вывода в консоли:

Hell0 w0rld

---

### Мои заметки:
- `replace(что_меняем, на_что_меняем)`
- Заменяет все вхождения, не только первое
- Работает с символами `replace('o', '0')` и со строками `replace("o", "0")`

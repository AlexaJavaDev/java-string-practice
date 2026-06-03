**Что делает:**  
Проходит по строке `"Hello"` от первого символа до последнего и выводит каждый символ с новой строки.

**Код:**
```java
    public static void main(String[] args) {
        String str = "Hello";
        System.out.println(loop(str));
    }

    public static String loop(String str) {
        String result = "";
        for (int i = 0; i < str.length(); i++) {
            result += str.charAt(i) + "\n";
        }
        return result;
    }
```
#### Пример вывода в консоли:

H  
e  
l  
l  
o  

### Мои заметки:
- `charAt(i)` — берёт символ по индексу `i`
- Индексы начинаются с `0`, а не с `1`

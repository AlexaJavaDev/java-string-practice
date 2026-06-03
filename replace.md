# Вариант 1: буква на цифру
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

# Вариант 2: буква на символ
**Что делает:**  
Заменяет все буквы "l" на символ "*" в строке "Hello world".

**Код:**
```java
    public static void main(String[] args) {
        String str = "Hello world";
        System.out.println(loop(str));
    }

    public static String loop(String str) {
        return str.replace("l", "*");
    }
```
#### Пример вывода в консоли:
He**o wor*d

---

# Вариант 3: убираем пробелы и выводим длину
**Что делает:**  
Убирает все пробелы из строки "Hello world" и выводит длину получившейся строки.

**Код:**
```java
    public static void main(String[] args) {
        String str = "Hello world";
        String res = str.replace(" ", "");
        System.out.println(res.length());
    }
```
#### Пример вывода в консоли:
10

---

# Вариант 4: все перечисленные буквы на символ

**Что делает:**  
Заменяет все гласные буквы (a, e, i, o, u) на символ "*" в строке "Hello".  
`(?i)` — означает, что регистр не важен (и заглавные, и строчные).

**Код:**
```java
    public static void main(String[] args) {
        String str = "Hello";
        System.out.println(str.replaceAll("(?i)[aeiou]", "*"));
    }
```
#### Пример вывода в консоли:
H * l l *

---

### Мои заметки:
`replace(что_меняем, на_что_меняем)`  
`replace(" ", "")` — убирает все пробелы (меняет пробел на пустоту)  
`replaceAll()` — заменить все  
`[aeiou]` — означает любую гласную букву  
`(?i)` — делает поиск нечувствительным к регистру  
`"l"` или `"*"` можно менять на любые символы или подстроки  
Регистр важен: `"L"` не заменит  
Работает с символами `replace('o', '0')` и со строками `replace("o", "0")`  
Так можно считать количество символов без пробелов  
Заменяет все вхождения, не только первое  

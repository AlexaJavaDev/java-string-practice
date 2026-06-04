## Вариант 1: первые 5 символов

**Что делает:**  
Выводит первые 5 символов строки "Программирование".

**Код:**
```java
    public static void main(String[] args) {
        String str = "Программирование";
        System.out.println(loop(str));
    }

    public static String loop(String str) {
        return str.substring(0, 5);
    }
```
#### Пример вывода в консоли:
```
Прогр
```

---

## Вариант 2: последние 5 символов
**Что делает:**  
Выводит последние 5 символов строки "Программирование".

**Код:**
```java
    public static void main(String[] args) {
        String str = "Программирование";
        System.out.println(loop(str));
    }

    public static String loop(String str) {
        return str.substring(str.length() - 5, str.length());
    }
```
#### Пример вывода в консоли:
```
вание
```

---

## Вариант 3: выводим строку от указанного символа
**Что делает:**  
Находит индекс первого вхождения буквы "w" в строке "Hello world" и выводит всё, начиная с этой позиции до конца строки.

**Код:**
```java
    public static void main(String[] args) {
        String str = "Hello world";
        System.out.println(str.substring(str.indexOf("w")));
    }
```

#### Пример вывода в консоли:
```
world
```

---

**Что происходит по шагам:**

| Шаг | Что делаем | Результат |
|-----|------------|-----------|
| 1	| `str.indexOf("w")` | ищем индекс `"w"` → возвращает `6` |
| 2	| `str.substring(6)` | выводим символы с индекса `6` до конца |
| 3	| Выводим результат | "world" |

---

**Другие примеры:**

```java
str.substring(str.indexOf("o"))     // "o world"
str.substring(str.indexOf("l"))     // "llo world"  (первое l на индексе 2)
str.substring(str.indexOf(" "))     // " world"     (начинается с пробела)
```

---

### Мои заметки:
- `substring(0, 5)` — берёт символы с индекса `0` до индекса `4` (5 не входит!)  
- `substring(индекс)` — вырезает часть строки с указанного индекса до конца  
- Формула: `substring(начало, конец)` — конец не включается  
- `indexOf(подстрока)` — ищет первое вхождение и возвращает его индекс  
- Вместе они работают так: `str.substring(str.indexOf("w"))` — "вырежи всё, до буквы w, остальное выведи"  
- Первые `N` символов = `substring(0, N)`
- Последние `N` символов = `substring(str.length() - N, str.length())`
- `str.length() - 5` — начало за `5` символов до конца
- `str.length()` — конец (последний индекс + 1)
- Если символ не найден, `indexOf()` вернёт `-1`, и `substring(-1)` вызовет ошибку (надо проверять)

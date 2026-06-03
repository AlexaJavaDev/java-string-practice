## Вариант 1: первые 5 символов

**Что делает:**  
Выводит первые 5 символов строки "Программирование".

**Код:**
```java
    public static void main(String[] args) {
        String str1 = "Программирование";
        System.out.println(loop(str1));
    }

    public static String loop(String str1) {
        return str1.substring(0, 5);
    }
```
#### Пример вывода в консоли:
Прогр

---

### Мои заметки:
- `substring(0, 5)` — берёт символы с индекса `0` до индекса `4` (5 не входит!)
- Формула: `substring(начало, конец)` — конец не включается
- Первые `N` символов = `substring(0, N)`

---

## Вариант 2: последние 5 символов
**Что делает:**  
Выводит последние 5 символов строки "Программирование".

**Код:**
```java
    public static void main(String[] args) {
        String str1 = "Программирование";
        System.out.println(loop(str1));
    }

    public static String loop(String str1) {
        return str1.substring(str1.length() - 5, str1.length());
    }
```
#### Пример вывода в консоли:
вание

---

### Мои заметки:
- `str1.length() - 5` — начало за `5` символов до конца
- `str1.length()` — конец (последний индекс + 1)
- Последние `N` символов = `substring(str.length() - N, str.length())`

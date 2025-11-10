

---

# Лабораторна робота №5 – Узагальнені типи, колекції, LINQ та винятки

## Опис проєкту

Цей проєкт демонструє роботу з:

* **Узагальненими класами та методами (Generics)**
* **Колекціями C#** (`List<T>`, з можливістю використання `Dictionary`, `HashSet`)
* **LINQ** для фільтрації та обчислень
* **Обробкою винятків** та створенням власних класів винятків

Проєкт містить приклад роботи зі студентами, де:

* Використовується **Repository<T>** для зберігання об’єктів типу `Student`
* Виконується **фільтрація студентів за оцінкою** через LINQ
* Демонструється **створення та обробка власного винятку `InvalidGradeException`**

---

## Структура проєкту

```
Lab5/
?? Program.cs                   # Головна програма з Main()
?? Repository.cs                # Узагальнений клас Repository<T>
?? Student.cs                   # Клас-модель Student
?? InvalidGradeException.cs     # Власний клас винятку
?? README.md                    # Опис проєкту
```

---

## Інструкція з запуску

1. Клонувати або завантажити проєкт.
2. Відкрити у Visual Studio або VS Code.
3. Переконатися, що встановлений **.NET 7.0** або новіший.
4. Відкрити `Program.cs` та запустити програму.
5. В консолі буде виведено:

* Студентів з оцінкою більше 80
* Повідомлення про виняток, якщо оцінка некоректна
* Повідомлення про завершення програми

---

## Особливості проєкту

* Підтримка **українських символів** у консолі:

```csharp
Console.OutputEncoding = System.Text.Encoding.UTF8;
Console.InputEncoding = System.Text.Encoding.UTF8;
```

* Легко розширюється для інших типів даних завдяки **узагальненому репозиторію**.
* Використання **LINQ** робить код чистим та зрозумілим.
* Приклад **власного винятку** демонструє правильну обробку помилок.

---

## Приклад виводу

```
Студенти з оцінкою більше 80:
Іван, Age: 20, Grade: 85
Оля, Age: 22, Grade: 92
Анна, Age: 21, Grade: 88
Власний виняток: Оцінка не може бути більше 100
Програма завершила виконання.
```

## Приклад запуску програми:
![Screen](image.png)

---

## Посилання на документацію

* [Generics in C#](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/types/generics)
* [Collections in C#](https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/collections)
* [LINQ in C#](https://learn.microsoft.com/en-us/dotnet/csharp/linq)
* [Exception Handling](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/exceptions/)

---
# 🛒 Автотесты для SauceDemo (Java + Selenium + TestNG)

Автоматизация тестирования демо-магазина [SauceDemo](https://www.saucedemo.com/).  
Проект для демонстрации навыков UI-автоматизации с использованием Page Object Model, TestNG и Allure.

---

## 📌 Что покрыто тестами

- ✅ Авторизация (позитивные и негативные сценарии)
- ✅ Добавление товаров в корзину
- ✅ Оформление заказа
- ✅ Проверка элементов каталога
- ✅ Проверка корзины

---

## 🛠️ Стек технологий

| Компонент | Технология |
| :--- | :--- |
| **Язык** | Java 17 |
| **Тестовый фреймворк** | TestNG |
| **UI-тестирование** | Selenium WebDriver |
| **Паттерн** | Page Object Model |
| **Сборка** | Maven |
| **Отчёты** | Allure |
| **CI/CD** | GitHub Actions |
| **Система контроля версий** | Git, GitHub |

---

## 📁 Структура проекта
src/
├── main/java/
│   ├── pages/          # Page Object'ы
│   └── utils/          # Утилиты
└── test/java/
└── tests/          # Тестовые классы
├── LoginTest
├── ProductsTest
├── CartTest
└── CheckoutTest

```

---

## 🚀 Как запустить

### 1. Клонировать репозиторий
```bash
git clone https://github.com/ваш-логин/Saucedemo.git
cd Saucedemo
```

2. Установить зависимости

```bash
mvn clean install
```

3. Запустить все тесты

```bash
mvn clean test
```

4. Открыть Allure-отчёт

```bash
mvn allure:serve
```

---

📊 Allure-отчёт

После запуска Allure формирует отчёт с шагами, скриншотами и временем выполнения тестов.

---

🧪 Пример теста

```java
@Test
public void loginTest() {
    loginPage.open();
    loginPage.enterUsername("standard_user");
    loginPage.enterPassword("secret_sauce");
    loginPage.clickLogin();
    Assert.assertEquals(productsPage.getTitle(), "Products");
}
```

---

📌 Планы по улучшению

· Добавить API-тесты (REST Assured)
· Настроить параллельный запуск
· Добавить логирование через Log4j

---

👤 Обо мне

Имя: Татьяна
Стажировка: Автоматизация тестирования (Java + Selenium + TestNG)
Стаж работы: 10 лет (в декрете)

🐙 GitHub: github.com/Liseikinatatiana

---

📜 Лицензия

Учебный проект. Все права на SauceDemo принадлежат их владельцам.


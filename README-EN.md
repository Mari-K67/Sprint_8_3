# Sprint_8
Task 1: Unit tests.  
Autotests to verify a program that helps order a burger in Stellar Burgers

## What you need to do
* Clone the [repository](https://github.com/Yandex-Practicum/qa-python-project) with code template.
* Connect libraries: pytest, pytest-cov. 
* Cover with tests the classes `Bun`, `Burger`, `Ingredient`, `Database`.
* Use mocks and parametrization where needed.
* Code coverage should not be lower than 70%.

---

## Task 2: API
Task: test the API endpoints for [Stellar Burgers](https://qa-stellarburgers.education-services.ru) ([API documentation](https://code.s3.yandex.net/qa-automation-engineer/python-full/diploma/api-Stelar_Burger_10.25.pdf?etag=3584917d935c90b69cb3ffaff58d4f34)).

## User creation:
* create a unique user;
* create a user who is already registered;
* create a user and do not fill in one of the required fields.

## User login:
* login as an existing user,
* login with an incorrect login and password.

## User data modification:
* with authorization,
* without authorization,

For both situations, you need to check that any field can be changed. For an unauthorized user — also that the system will return an error.

## Order creation:
* with authorization,
* without authorization,
* with ingredients,
* without ingredients,
* with incorrect ingredient hash.

## Getting orders for a specific user:
* authorized user,
* unauthorized user.

**What you need to do:**
- Create a separate repository for API tests.
- Connect libraries: pytest, requests and allure-pytest.
- Write tests.
- Create a report in Allure.

---

## Task 3: Web application.
Task: test the web application [Stellar Burgers](https://qa-stellarburgers.education-services.ru).

**What you need to do:**
* Describe the elements that will be used in tests using the Page Object Model pattern.
* Test functionality in Google Chrome and Mozilla Firefox.
* Connect Allure report.

## Scenarios:
### Password recovery
Check:
* transition to the password recovery page by clicking the "Восстановить пароль" button,
* entering email and clicking the "Восстановить" button,
* clicking the show/hide password button makes the field active — highlights it.

### Personal account
Check:
* transition by clicking on "Личный кабинет",
* transition to the "История заказов" section,
* logout from account.

### Checking main functionality
Check:
* transition by clicking on "Конструктор",
* transition by clicking on "Лента заказов",
* if you click on an ingredient, a popup window with details will appear,
* the popup window closes by clicking the X button,
* when adding an ingredient to an order, the counter for this ingredient increases,
* a logged-in user can place an order.

### "Лента заказов" section
Check:
* if you click on an order, a popup window with details will open,
* user orders from the "История заказов" section are displayed on the "Лента заказов" page,
* when creating a new order, the "Выполнено за всё время" counter increases,
* when creating a new order, the "Выполнено за сегодня" counter increases,
* after placing an order, its number appears in the "В работе" section.

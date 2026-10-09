# Sprint_8
Task 3: Web application.
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

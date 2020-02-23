# **План автоматизации тестирования возможности открытия вклада "Накопилка".**
## Позитивные сценарии:
**Ввод валидных данных через меню "Вклады"**

1. Перейти на сайт https://alfabank.ru
2. Нажать на вкладку "Вклады" 
3. Нажать на вкладку "Накопительные счета"
4. Нажать на блок "Накопилка" 
5. Нажать на кнопку "Заполнить заявку" 
6. Заполнить поля "Имя" и "Мобильный телефон" валидными данными (Имя:Наталья, Мобильный телефон: +7(922)523-46-79)
7. Нажать на чек-бокс "Я согласен(а) на обработку персональных данных"
8. Нажать на кнопку "Мы перезвоним"
Ожидаемый результат:
Появится сообщение "Спасибо, скоро мы вам перезвоним!"

**Ввод валидных данных через меню "Накопилка"**

1. Перейти на сайт https://alfabank.ru
2. Нажать на вкладку "Частным лицам" 
3. Навести курсор на меню "Вклады"
4. Нажать на вкладку "Накопилка" 
5. Нажать на кнопку "Заполнить заявку" 
6. Заполнить поля "Имя" и "Мобильный телефон" валидными данными (Имя:Наталья, Мобильный телефон: +7(922)523-46-79)
7. Нажать на чек-бокс "Я согласен(а) на обработку персональных данных"
8. Нажать на кнопку "Мы перезвоним"

Ожидаемый результат
Появится сообщение "Спасибо, скоро мы вам перезвоним!"

## Негативные сценарии
**Попытка отправить форму с незаполненном полем "Имя"**

1. Перейти на сайт https://alfabank.ru
2. Нажать на вкладку "Частным лицам" 
3. Навести курсор на меню "Вклады"
4. Нажать на вкладку "Накопилка" 
5. Нажать на кнопку "Заполнить заявку" 
6. Поле "Имя" оставить пустым
6. Заполнить поле "Мобильный телефон" валидными данными (Мобильный телефон: +7(922)523-46-79)
7. Нажать на чек-бокс "Я согласен(а) на обработку персональных данных"
8. Нажать на кнопку "Мы перезвоним"

Ожидаемый результат
Появится сообщение "Это поле обязательно для заполнения!"

**Попытка отправить форму с незаполненном полем "Мобильный телефон"**

1. Перейти на сайт https://alfabank.ru
2. Нажать на вкладку "Частным лицам" 
3. Навести курсор на меню "Вклады"
4. Нажать на вкладку "Накопилка" 
5. Нажать на кнопку "Заполнить заявку" 
6. Заполнить поле "Имя" валидными данными (Имя: Наталья)
6. Полее "Мобильный телефон" оставить пустым
7. Нажать на чек-бокс "Я согласен(а) на обработку персональных данных"
8. Нажать на кнопку "Мы перезвоним"
Ожидаемый результат
Появится сообщение "Это поле обязательно для заполнения!"

**Попытка отправить форму, когда в поле "Имя" введены цифры**
1. Перейти на сайт https://alfabank.ru
2. Нажать на вкладку "Частным лицам" 
3. Навести курсор на меню "Вклады"
4. Нажать на вкладку "Накопилка" 
5. Нажать на кнопку "Заполнить заявку" 
6. Ввести в поле "Имя" цифры (Имя: 34567898765)
6. Заполнить поле "Мобильный телефон" валидными данными (Мобильный телефон: +7(922)523-46-79)
7. Нажать на чек-бокс "Я согласен(а) на обработку персональных данных"
8. Нажать на кнопку "Мы перезвоним"

Ожидаемый результат
Появление сообщения "Значение поля может содержать только буквы и дефис"

**Попытка отправить форму, когда в поле "Имя" поставили один пробел**
1. Перейти на сайт https://alfabank.ru
2. Нажать на вкладку "Частным лицам" 
3. Навести курсор на меню "Вклады"
4. Нажать на вкладку "Накопилка" 
5. Нажать на кнопку "Заполнить заявку" 
6. Поставить в поле "Имя" один пробел
6. Заполнить поле "Мобильный телефон" валидными данными (Мобильный телефон: +7(922)523-46-79)
7. Нажать на чек-бокс "Я согласен(а) на обработку персональных данных"
8. Нажать на кнопку "Мы перезвоним"

Ожидаемый результат
Появление сообщения "Значение поля должно содержать больше одной буквы"

**Попытка отправить форму с не полностью заполненным полем "Мобильный телефон"**

1. Перейти на сайт https://alfabank.ru
2. Нажать на вкладку "Частным лицам" 
3. Навести курсор на меню "Вклады"
4. Нажать на вкладку "Накопилка" 
5. Нажать на кнопку "Заполнить заявку" 
6. Заполнить поле "Имя" валидными данными (Имя: Наталья)
6. Заполнить поле "Мобильный телефон" не полностью (Мобильный телефон: +7(922)523)
7. Нажать на чек-бокс "Я согласен(а) на обработку персональных данных"
8. Нажать на кнопку "Мы перезвоним"
Ожидаемый результат
Появление сообщения "Проверьте, пожалуйста, номер телефона!"

## **Используемые инструменты:**
* Java 8. Кросс-платформенная совместимость, автоматическое управление памятью, распространённость.
* IntelliJ IDEA. Интегрированная среда для написания тестов. Умное автодополнение, анализ кода в реальном времени и надежные рефакторинги.
* Junit-jupiter 5.5.1. Возможность создавать параметризованные тесты.
* Selenide 5.3.1. Автоматическое управление браузером, более удобный синтаксис чем у Selenium.
* Faker. Генерирует уникальные данные.
* Allure. Наглядные отчёты.
## **Перечень и описание возможных рисков при автоматизации**
* Возникновение проблем с запуском контейнеров и SUT.
* Отсутствие ТЗ.
* Нехватка времени.

## **Перечень необходимых разрешений/данных/доступов от банка**
* Разрешение на тестирование продукта.
* Спецификация на тестируемый продукт.
* Разрешение и доступ к заглушке БД.
## **Интервальная оценка с учётом рисков (в часах)**
25 человекочасов.
## **Перечень необходимых специалистов для автоматизации**
* Тестировщик со знанием автоматизации процесса тестирования.
* Разработчик продукта.

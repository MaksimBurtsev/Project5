## Страница 1. "Выбор полиса"


| Описание                                      | Xpath                                                                                    |
|-----------------------------------------------|------------------------------------------------------------------------------------------|
| Кнопка "Квартира"                              | //mat-button-toggle[@id='mat-button-toggle-1'] или //button[contains(.,"Квартира")]     |
| Сдаётся в аренду (квартира)                    |                                                                                         |
| Кнопка “Да”                                    | //div[text()='Сдается в аренду']/following::mat-button-toggle[1] или //*[text()='Сдается в аренду']/following::button[1]                     |
| Кнопка "Heт"                                   | //div[text()='Сдается в аренду']/following::mat-button-toggle[1] или //*[text()='Сдается в аренду']/following::button[2]                     |
| Расположена на первом или последнем этаже      |                                                                                         |
| Кнопка “Да”                                    | //div[text()='Расположена на первом или последнем этаже']/following::mat-button-toggle[1] или //*[text()='Расположена на первом или последнем этаже']/following::button[1]                |
| Кнопка “Нет”                                   | //div[text()='Расположена на первом или последнем этаже']/following::mat-button-toggle[1] или //*[text()='Расположена на первом или последнем этаже']/following::button[2]   |
| Установлена охранная сигнализация (квартира)   |                                                                                         |
| Кнопка "Да"                                    | //div[text()='Установлена охранная сигнализация']/following::mat-button-toggle[1] или //*[text()='Установлена охранная сигнализация']/following::button[1] или //h4[text()='Особенности объекта']/following::mat-button-toggle[5]     
| Кнопка "Нет"                                   | //div[text()='Установлена охранная сигнализация']/following::mat-button-toggle[2] или //*[text()='Установлена охранная сигнализация']/following::button[2] или //h4[text()='Особенности объекта']/following::mat-button-toggle[6]   
| Применить                                      | //button[contains(@class, 'action-back')] или //button[contains(.,"Применить")]          |
| Оформить                                       | //button[@color='accent' or contains(@class, 'mat-button-disabled')]                     |
| Кнопка "Дом"                                   | //mat-button-toggle[@id='mat-button-toggle-2']                                           |
| Сдаётся в аренду (дом)                         |                                                                                          |
| Кнопка "Да"                                    | //div[text()='Сдается в аренду']/following::mat-button-toggle[1] или //*[text()='Сдавется в аренду']/following::button[1] |
| Кнопка "Нет"                                   | //div[text()='Сдается в аренду']/following::mat-button-toggle[2] или //*[text()='Сдавется в аренду']/following::button[2] |
| Установлена охранная сигнализация (дом)        |                                                                                          |
| Кнопка "Да"                                    | //div[text()='Установлена охранная сигнализация']/following::mat-button-toggle[1] или //*[text()='Установлена охранная сигнализация']/following::button[1] |
| Кнопка "Нет"                                   | //div[text()='Установлена охранная сигнализация']/following::mat-button-toggle[2] или //*[text()='Установлена охранная сигнализация']/following::button[2] |
| Материал несущих стен                          |                                                                                          |
| Кнопка "Кирпич или монолит"                    | //h4[text()='Особенности объекта']/following::mat-button-toggle[5] или //*[text()=' Кирпич или монолит ']/ancestor::button                                              |
| Кнопка "Дерево"                                | //h4[text()='Особенности объекта']/following::mat-button-toggle[6] или //*[text()=' Дерево ']/ancestor::button                               |


## Страница 2. "Оформление"


| Заголовок | Название                            | Xpath                                                      |
| --------- | ----------------------------------- | ---------------------------------------------------------- |
| Кнопки    | Заполнить по Сбер ID                | //button[@color="primary"] или //button[contains(.,"Заполнить по Сбер ID")]                                |
|           | Мужской                             | //button[@name="mat-button-toggle-group-57"][@aria-pressed="true"] или //button[contains(.,"Мужской")]     |
|           | Женский                             | //button[@name="mat-button-toggle-group-57"][@aria-pressed="false"] или //button[contains(.,"Женский")]    |
|           | Вернуться                           | //button[contains(@class, "action-back")]                   |
|           | Оформить                            | //button[@color="accent"] или //button[contains(@class, 'mat-accent')] или //button[contains(.,"Оформить")]|
                                                                           




| Заголовок   | Название                                       | Xpath                                                       |
| ----------- | ---------------------------------------------- | ----------------------------------------------------------- |
| Поля для    | Фамилия                                        | //div[@class="mat-form-field-flex ng-tns-c61-4"] или //input[@formcontrolname="lastName"]                           | 
| ввода текста| Имя                                            | //div[@class="mat-form-field-flex ng-tns-c61-5"] или //input[@formcontrolname="name"]                               |
|             | Отчество                                       | //div[@class="mat-form-field-flex ng-tns-c61-6"] или //input[@formcontrolname="middleName"]                         |
|             | Серия                                          | //div[@class="mat-form-field-flex ng-tns-c61-8"] или //input[@formcontrolname="docSeries"]                          |
|             | Номер                                          | //div[@class="mat-form-field-flex ng-tns-c61-9"] или //input[@formcontrolname="docNumber"]                          |
|             | Кем выдан                                     | //div[@class="mat-form-field-flex ng-tns-c61-11"] или //textarea[@formcontrolname="docIssuer"]                       |
|             | Код подразделения                             | //div[@class="mat-form-field-flex ng-tns-c61-12"] или //input[@formcontrolname="docDepartmentCode"                   |
|             | Регион проживания                             | //div[@class="mat-form-field-flex ng-tns-c61-12"] или //input[@formcontrolname="registrationRegion"] или //*[text()='Регион проживания']/ancestor::mat-form-field        |
|             | Регион проживания 2                           | //div[@class="mat-form-field-flex ng-tns-c61-0"]  или //input[@formcontrolname="registrationRegion"]                 |
|             | Город или населенный                          | //div[@class="mat-form-field-flex ng-tns-c61-14"] или //input[@formcontrolname="registrationCity"]                   |
|             | Улица                                          | //div[@class="mat-form-field-flex ng-tns-c61-15"] или //input[@formcontrolname="registrationStreet"]                |
|             | Дом, литера, корпус, строение                 | //div[@class="mat-form-field-flex ng-tns-c61-16"] или //input[@formcontrolname="registrationHouse"]                  |
|             | Квартира                                       | //div[@class="mat-form-field-flex ng-tns-c61-17"] или //input[@formcontrolname="registrationFlat"]                  |
|             | Телефон                                        | //div[@class="mat-form-field-flex ng-tns-c61-18"] или //input[@formcontrolname="contactPhone"]                      |
|             | Электронная почта                              | //div[@class="mat-form-field-flex ng-tns-c61-19“]  или //input[@formcontrolname="contactEmail"]                     |
|             | Повтор электронной почты                      | //div[@class="mat-form-field-flex ng-tns-c61-20"] или //input[@formcontrolname="repeatEmail"]                        |
|             | Промокод                                      | //input[@formcontrolname="promoCode"]                                                                                |
| Чекбоксы    | Улица отсутствует                             | //*[@id="mat-checkbox-2"] или //input[@id="mat-checkbox-2-input"]                                                    |
|             | Отчество отсутствует                          | //*[@id="mat-checkbox-1"] или //input[@id="mat-checkbox-1-input"]                                                    |
| Датапикеры  | Дата начала                                   | input[@formcontrolname="startDate"] или //*[@class="mat-datepicker-toggle-default-icon ng-star-inserted"]            |
|             | Дата рождения                                 | //div[@class="mat-form-field-flex ng-tns-c61-7"] или //*[text()='Дата рождения']/following::mat-datepicker-toggle[1] |
|             | Дата выдачи                                   | //div[@class="mat-form-field-flex ng-tns-c61-10"] или //*[text()='Дата выдачи']/following::mat-datepicker-toggle[1]  |
| Логотип     | "СБЕР СТРАХОВАНИЕ"                            | //div[@class="sber-logo"]                                                                                            |
| Слайдер     | Слайдер расположенный в блоке, предназначенном | //mat-slider или //div[@class="mat-slider-wrapper"]                                                                 |
|             | для выбора суммы                              |                                                                                                                      |
| Хедер       | Хедер "Что будет застраховано"                | //h4[@class="block-header"][1] или //h4[text() = "Что будет застраховано?"]                                          |
| Колонки "СЗ"| Левый                                         | //div[text() = "Чрезвычайная ситуация"]/ancestor::ul или //*[text()='Чрезвычайная ситуация']/ancestor::ul            |
|             | Правый                                        | //div[text() = "Стихийные бедствия"]/ancestor::ul  или  //*[text()='Стихийные бедствия']/ancestor::ul                |
| Текстовые   | Мебель, техника и ваши вещи                   | //div[contains(text(),'Мебель')]                                                                                     |
| блоки       | Падение летательных аппаратов                 | //div[text()="Падение летательных аппаратов и их частей"] или //*[text()='Падение летательных аппаратов и их частей']|
| Footer      | Футер                                         | //footer                                                                                                             |
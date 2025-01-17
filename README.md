# Домашнее задание по теме "Шаблонизатор Jinja 2."
## Цель: научиться взаимодействовать с шаблонами Jinja 2 и использовать их в запросах.

## Задача "Список пользователей в шаблоне":
**Подготовка:**

>1.Используйте код из предыдущей задачи.
>   
>2.Скачайте [***заготовленные шаблоны***](https://uguide.ru/tablica-osnovnykh-tegov-html-s-primerami)  для их дополнения.
>
>3.Шаблоны оставьте в папке ***templates***> у себя в проекте.
>
>4.Создайте объект **Jinja2Templates**, указав в качестве папки шаблонов - **templates**.

***Измените и дополните ранее описанные CRUD запросы:***

**Напишите новый запрос по маршруту '/':**

>1.Функция по этому запросу должна принимать аргумент ***request*** и возвращать **TemplateResponse.**
>
>2.**TemplateResponse** должен подключать ранее заготовленный шаблон ***'users.html'***, а также передавать в него ***request*** и список ***users***.
 Ключи в словаре для передачи определите самостоятельно в соответствии с шаблоном.
>
**Измените get запрос по маршруту '/user' на '/user/{user_id}':**

>1.Функция по этому запросу теперь принимает аргумент ***request*** и ***user_id***.
>
>2.Вместо возврата объекта модели **User**, теперь возвращается объект ***TemplateResponse***.
>
>3.***TemplateResponse*** должен подключать ранее заготовленный шаблон ***'users.html'***, а также передавать в него ***request** и одного из пользователей - ***user***.
> Ключи в словаре для передачи определите самостоятельно в соответствии с шаблоном.

**Создайте несколько пользователей при помощи post запроса со следующими данными:**
>1.username - UrbanUser, age - 24
>
>2.username - UrbanTest, age - 22
>
>3.username - Capybara, age - 60

В шаблоне ***'users.html'*** заготовлены все необходимые теги и обработка условий, вам остаётся только дополнить закомментированные строки вашим Jinja 2 кодом (использование полей id, username и age объектов модели User):
1. По маршруту '/' должен отображаться шаблон 'users.html' со списком все ранее созданных объектов:

   ![image](https://github.com/user-attachments/assets/e90c1a79-8b47-48a8-bd74-df4ac3fe0daa)

3. Здесь каждая из записей является ссылкой на описание объекта, информация о котором отображается по маршруту '/user/{user_id}':

  ![image](https://github.com/user-attachments/assets/e74bcdbc-3481-4273-a682-dc4d806a3ca2)


**Так должен выглядеть Swagger:**

![image](https://github.com/user-attachments/assets/5fae0364-0a70-4fb7-889f-29dd3d2feed2)


**Иерархия в проекте:**

![image](https://github.com/user-attachments/assets/65d4fcdb-ac77-4249-9107-d7f9cfc28041)


**Примечания:**
[Основные теги HTML](https://uguide.ru/tablica-osnovnykh-tegov-html-s-primerami)

**Файл module_16_5.py, шаблоны main.html и users.html загрузите на ваш GitHub репозиторий. В решении пришлите ссылку на него.**

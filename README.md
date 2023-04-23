# Домашнее задание к занятию "12.1 «Базы данных»" - Евгений Шахов
---
### Задание 1

Create table Сотрудники *(  
id int  
Фамилия varchar (50) not null,  
Имя varchar (50) not null,  
Отчество varchar (50) not null,  
Оклад numeric,  
Должность внешний ключ,  
Структурное подразделение внешний ключ,  
Дата найма date,  
Проекты внешний ключ,  
)*  

Create table Филиалы *(  
id int  
Адрес varchar (200) not null,  
Структурное подразделение внешний ключ,  
)*  

Create table Структурное подразделение *(  
id int  
Тип подразделения внешний ключ,  
Наименование подразделения varchar (100) not null,  
)*  

Create table Тип подразделения *(  
id int  
Тип подразделения varchar (50) not null,  
)*  

Create table Проекты *(  
id int  
Наименование проекта varchar (100) not null,  
Сотрудники внешний ключ,  
)*  

Create table Должности *(  
id int  
Структурное подразделение внешний ключ,  
Наименование должности varchar (50) not null,  
)*  

Create table Зарплатная ведомость *(  
id int  
Сотрудники внешний ключ,  
Оклад numeric,  
)*  

Create table Премирование *(  
id int  
Сотрудники внешний ключ,  
Размер премии numeric,  
)*  

---

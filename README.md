# Домашнее задание к занятию "12.1 «Базы данных»" - Евгений Шахов
---
### Задание 1

Create table Сотрудники *(  
id int  
Фамилия varchar (50) not null,  
Имя varchar (50) not null,  
Отчество varchar (50) not null,  
Оклад numeric,  
Должность varchar (50) not null,  
Дата найма date,  
)*

Create table Организационная структура *(  
id int  
Тип подразделения varchar (50) not null,  
Структурное подразделение varchar (100) not null,  
)*  

Create table Филиалы *(  
id int  
Регион varchar (150) not null,  
Город varchar (100) not null,  
Улица varchar (100) not null,  
Номер дома numeric,  
)*  

Create table Проекты *(  
id int  
ФИО сотрудника varchar (150) not null,  
Проект varchar (100) not null,  
)*  

Create table Заработная плата *(  
id int  
Структурное подразделение varchar (100) not null,  
Должность varchar (50) not null,  
Оклад numeric,  
)*  

Create table Должности *(  
id int  
Наименование должности varchar (50) not null,  
Структурное подразделение varchar (100) not null,  
)*  

Create table Зарплатная ведомость *(  
ФИО сотрудника varchar (150) not null,  
Оклад numeric,  
)*  

---

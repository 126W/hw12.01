# Домашнее задание к занятию "12.1 «Базы данных»" - Евгений Шахов
---
### Задание 1

Create table Сотрудники *(  
id int  
ФИО varchar (150) not null,   
Оклад numeric,  
Должность varchar (50) not null,  
Структурное подразделение внешний ключ,  
Дата найма date,   
)*  

Create table Филиалы *(  
id int  
Адрес varchar (200) not null,  
Структурное подразделение внешний ключ,   
Проекты внешний ключ,   
)*  

Create table Структурное подразделение *(  
id int  
Тип подразделения varchar (50) not null,  
Наименование подразделения varchar (100) not null,   
)*   

Create table Проекты *(  
id int  
Проект varchar (100) not null,   
ФИО внешний ключ,   
)*  

Create table Должности *(  
id int  
Структурное подразделение внешний ключ,     
Наименование должности varchar (50) not null,    
)*  

Create table Зарплатная ведомость *(  
id int  
ФИО внешний ключ,    
Оклад numeric,      
)*  

Create table Премирование *(  
id int  
ФИО внешний ключ,  
Размер премии numeric,  
)*  

---

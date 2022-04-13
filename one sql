create database taskone
use taskone
create table Students
(
 Id int primary key identity,
 Name nvarchar(20) not null,
 Surname nvarchar(20)not null,
 GroupId int
)
create table StudentExsams
(
 Id int primary key identity,
 StudentId int ,
 ExsamId int ,
 Result int 
)
insert into Students(name,Surname,GroupId)
values 
('Azad','huseynov',2),
('hesen','memmedov',3),
('muraad','alizade',4),
('nahid','mirzeyev',5),
('muqeddes','cavadzade',1)
insert into StudentExsams(StudentId,ExsamId,Result)
values
(2,1,30),
(1,2,50),
(3,3,40),
(4,4,10),
(5,5,20)
create table Groups
(
 Id int primary key identity,
 No nvarchar(10) not null
)
create table Exsams
(
 Id int primary key identity,
 StudentexsamcountId int,
 Date datetime2
)
create table Subjects
(
 Id int primary key identity,
 No nvarchar(10) not null
)
insert into Subjects
values
('nahid'),
('Azad'),
('ali'),
('memmed'),
('rasim')
insert into Groups
values
('AP201'),
('AP202'),
('AP203'),
('AP204'),
('AP205')
select*from Students
join Groups on Students.GroupId=Groups.Id
insert into Exsams(StudentexsamcountId,Date)
values
(2,'2015-1-1'),
(1,'2013-2-5'),
(3,'2012-4-6'),
(5,'2019-5-8'),
(4,'2017-8-9')
select*from Students
join Exsams on Students.Id=Exsams.Id 
select*from Subjects
join Exsams on StudentexsamcountId<1

select Students.name+' '+Students.surname as 'fullname' from Students 
join Exsams on StudentexsamcountId>0

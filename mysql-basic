-- Show Database --
SHOW DATABASES;

-- Create Database --
CREATE DATABASE bookstore1;

-- Use Database --
USE bookstore1;

-- Show Table --
SHOW tables;

-- Create Table --
create table books ( id int auto_increment primary key, 
author1 varchar(100) not null, 
author2 varchar(100), 
author3 varchar(100), 
title varchar(100), 
description varchar(100), 
place_sell varchar(3), 
stock int default 0, 
creation_date datetime  default  current_timestamp  on update current_timestamp );

-- Update Table --
Alter table books 
add price int default 0,
status enum('available','out of stock','limited');

-- Delete Table --
alter table books drop place_sell;

-- Insert Table --
insert into books(author1, author2, author3, title, description, stock, creation_date, price, status) values('garnedyna','gareen','nana','cinta datang terlambat','based on true story, wanita yang jatuh cinta terlambat ketika ia sudah dengan yang lain',100,'2019/04/24 16:30:45',100000,'limited'),
 ('Rafael','Prawira','Diharja','cinta terhalang restu','based on true story, 2 insan yang slaing mencintai namun terhalang oleh restu dari ibu pihak lakinya',100,'2016/03/03 20:11:10',100000,'available'),
('Kiandra','Putri','Prawira','My lovely Family','pentingnya parenting dalam mendidik anak',100,'2027/05/06 10:15:50',100000,'available');

-- Select Table --
select * from books;

-- Alias --
SELECT id as ID, author1 as A1, author2 as A2, author3 as A3
FROM books;

-- Select Where --
select * from books where ID = 1;

-- Operator AND --
select * from books where ID = 1 and author1 = 'garnedyna' ;

-- Operator OR --
select * from books where ID = 1 or author2 = 'rafael' ;

-- Operator NOT --
select * from books where not ID = 3; 

--- Order By ---
select * from books order by id asc;

--- Limit ---
select * from books
    -> limit 2;

--- Update ---
update books
set author1 = 'vousemevoyez', price = 125000
where id = 1;

--- Delete Row ---
delete from books where id = 2;
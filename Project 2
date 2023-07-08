create database BooksDB;
use BooksDB;
create table Books(
serial_no int primary key,
book_title varchar(30),
author_name varchar(30),
genre varchar(20),
publication int,
price int);

drop table Books;

create table authors(
s_no int primary key,
author_age int,
author_native varchar(50),
author_name varchar(60),
serial_no int,
constraint fk_serial_no foreign key(serial_no) references Books(serial_no) 
ON DELETE SET NULL );


insert into Books values(1,"Cindrella","Walter Elias Disney","Cartoon",1997,5000);
insert into Books values(2,"Zombie","Hitler","Horror",1987,500);
insert into Books values(3,"Life of Pie","Mary Comb","Life lesson",2007,2000);
insert into Books values(4,"Life of Lord","Prince Jack","Fiction",1907,4000);
insert into Books values(5,"World tour","William","action",2002,5500);
insert into Books values(6,"Poppins","Wright Brothers","Cartoon",2010,3000);

insert into authors values(1,20,"Dubai","William",5);
insert into authors values(2,25,"Bombay","Hitler",2);
insert into authors values(3,30,"Sidney","Walter Elias Disney",1);
insert into authors values(4,40,"Darjiling","Wright Brothers",6);


drop table Books;
drop table authors;

select * from Books;
select * from authors;

select * from Books
where book_title = "Cindrella";

select * from Books
where book_title Like 'life%';

update Books
set price = '10000'
where book_title = "Life of Pie";

delete from Books
where book_title = "Zombie";

select avg(price)
from Books;

-- inner join: only matching rows
SELECT * FROM Books
INNER JOIN authors
ON Books.serial_no=authors.serial_no
ORDER BY s_no;

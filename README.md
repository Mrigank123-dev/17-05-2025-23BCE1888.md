show databases ;
use school;

create table student(
	student_id int,
    student_name varchar(40),
    student_department varchar(40),
    student_age int
);

insert into student values(123,"Miraak","Conjuration",345);
insert into student values(124,"Conq","Restoration",34);
insert into student values(125,"Eijya","Conjuration",34567);
insert into student values(126,"Twinx","Destruction",399);

desc teacher ;

alter table student add(
	student_address varchar(40)
);
alter table student drop column student_address ;

alter table student add(
	student_address varchar(40) default 'Bityora'
    );
insert into student values('234','nenya','Healing',45);
select * from student ;
update student set age=age+1000 ;
update student set student_address="Ongrola" where student_id=123;
desc student ;
select * from student ;

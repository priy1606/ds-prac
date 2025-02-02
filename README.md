Create keyspace keyspace1 with replication = { 'class':'SimpleStratergy','replication_factor': '3' }; Create table dept ( dept_id int PRIMARY KEY, dept_name text, dept_loc text);
Create table emp ( emp_id int PRIMARY KEY, emp_name text, dept_id int,email text, phone text ); Insert Queries for dept table
Insert into dept (dept_id, dept_name, dept_loc) values (1001,'Accounts', 'Mumbai'); Insert into dept (dept_id, dept_name, dept_loc) values (1002,'Marketing', 'Delhi'); Insert into dept (dept_id, dept_name, dept_loc) values (1003, 'HR','Chennai'); Insert Queries for emp table
Insert into emp ( emp_id, emp_name, dept_id, email, phone ) values (1001, 'ABCD',1001, 'abcd@company.com', '1122334455');
Insert into emp ( emp_id, emp_name, dept_id, email, phone ) values (1002, 'DEFG',1001, 'defg@company.com', '2233445566');
Insert into emp ( emp_id, emp_name, dept_id, email, phone ) values (1003, 'GHIJ',1002, 'ghij@company.com', '3344556677');
Insert into emp ( emp_id, emp_name, dept_id, email, phone ) values (1004, 'JKLM',1002, 'jklm@company.com', '4455667788');
Insert into emp ( emp_id, emp_name, dept_id, email, phone ) values (1005, 'MNOP',1003, 'mnop@company.com', '5566778899');
Insert into emp ( emp_id, emp_name, dept_id, email, phone ) values (1006, 'MNOP',1003, 'mnop@company.com', '5566778844');
Select-all Query for emp table select * from emp
Select-all Query for dept table select * from dept
Update query for dept table where dept_id=1003 set dept_name is Human Resource update dept set dept_name='Human Resource' where dept_id=1003;
Delete query for emp table where emp_id=1006 and Select-all from emp delete from emp where emp_id=1006;
select * from emp

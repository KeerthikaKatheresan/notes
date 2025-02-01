# notes

git bash required -connect my machine to cloud
github.com->create your own account
git init->create a folder in your system
git commit
git add->to move from working directory to staging Index
git add .->to add all file at once
git add filename path->to add specific file

git config user.username->only first time
push command->git push origin path_of_github_account

to see about project->git log
git status

git commit -m"<Message>"
git push
git push -u origin git_hub_acc path origin master->to push all file sto repository
git branch<branch-name>->to create a new branch
git branch or git branch --list->to find which branch we are in 
git checkout new _branch_name ->to checkout from one branch and move to another branch
git branch <name-of-branch-to-merge-in>
git pull->pull the updated project in your system
git log

angular,java springboot,mysql,


Group id:
artifact id->projrct name(sample_project)
package shows the path hirerachy


system info->system name

open git bash
1.git status
2.git init
3.git add
5.config your username and email
4.git commit
6. git remote add origin https://github.com/KeerthikaKatheresan/sample_repository.git
7.git push -u origin master
rm -rf .git


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
DataBase
1.DDL
2.DML-UPDATE 
3.Query language-select
4.Where clause
5.Alter 
truncate vs delete
alter vs modify
6.TCL -Always used with DML 
7.Checkpoint,save point
8.Constraint
9.Table level constraint ,column level constraint
how to use check comstraint after creation of table->homework
create 2 table with foreign key and use constrain and try voilating it
how to add cascade command in parent table(important 
Command 1:
create table empl(empid number(6),last_name varchar2(25) not null,Salary number(10),dept_id number(5),
constraint dept_fk foreign key(dept_id) references department (dept));

-------------------------------------------------------------------------------------------

-- create
CREATE TABLE EMPLOYEE (
  empId INTEGER PRIMARY KEY,
  name TEXT NOT NULL,
  dept TEXT NOT NULL
);

-- insert
INSERT INTO EMPLOYEE VALUES (0001, 'Clark', 'Sales');
INSERT INTO EMPLOYEE VALUES (0002, 'Dave', 'Accounting');
INSERT INTO EMPLOYEE VALUES (0003, 'Ava', 'Sales');

-- fetch 
SELECT * FROM EMPLOYEE WHERE dept = 'Sales';
select * from employee where empId=001;

create table company(
company_name TEXT,
reference_id int,
constraint fk_refer foreign key(reference_id)
references employee(empId) on delete cascade
);

insert into company values("Mphais",001);
insert into company values("Mphasis",002);
insert into company values("CisCo",003);

select * from company;
-----------------------------------------------------------------------------------
Normalization:
	Deletion Anamoly and pitfall
1NF,2NF,3NF
1NF:
	Table data should be atomic imp-atomic(futher decompose)
2nf:
	Non primary attribute cannot be partialy dependent
super key -combination of more than on primary key that can be used to fetch data

3NF:
	No trasitive dependency
a->b b->c a->c
	no column should be dependent upon another column in a transitive manner
BCNF:
	Super key should be primary key
	More strict about super key
-------------------------------------------------------------------------------------------




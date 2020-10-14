# part 1 

![Image of map](/commands.PNG)

## centos release check
![Image of map](/centos%20release.PNG)

## show os file capacity
![Image of map](/show%20file%20capa.PNG)

## list yum repolist
![Image of map](/list%20yum%20repo%20list.PNG)

## training passwd list
![Image of map](/training%20passwd%20list.PNG)

## list group skcc
![Image of map](/list%20group%20skcc.PNG)

## getent group skcc
![Image of map](/getent%20group%20skcc.PNG)

## getent passwd training
![Image of map](/getent%20passwd%20training.PNG)

## show databases
![Image of map](/show%20databases.PNG)

## show db version
![Image of map](/show%20db%20version.PNG)

## show db hostname
![Image of map](/show%20db%20hostname.PNG)

## cluster 구성
![Image of map](/cluster%20구성.PNG)

## cluster config
![Image of map](/cluster%20db%20config.PNG)

## create mysql user
![Image of map](/create%20mysql%20user.PNG)

## show authors, posts file in hue
![Image of map](/authors%20in%20hue.PNG)

## post, authors in hue
![Image of map](/posts%20in%20hue.PNG)

![Image of map](/hive%20authors%20posts.PNG)







# part 2
### num 1
select account.id, account.type, account.status, account.ammount, (account.ammount - avg(account.ammount) over (partition by account.type)) from account where account.status = 'Active'

### num 2
create external table employee (id INT, fname string, lname string, address string, city string, state string, zip string, birthday string, hireday string) stored as parquet location '/user/training/problem2/data/employee/'
![Image of map](/p2.PNG)
### num 3
create table solution as select c.id as id, c.fname as fname, c.lname as lname, c.hphone as hphone from customer c join account a on (c.id = a.custid) where a.amount < 0
![Image of map](/p3-2.PNG)

### num 4
hadoop fs -text /user/training/problem4/data/employee1 | hadoop fs -put - /user/training/problem5/data/employee2

### num 7
select concat(employee.fname, ' ', employee.lname) as fullname from employee where employee.city = 'Seattle'
![Image of map](/p7.PNG)

### num 8
sqoop export  --connect jdbc:mysql://localhost/problem8 --username cloudera --password cloudera --table solution --export-dir /user/training/problem8/data/customer/ -m 1

### num 9
alter table customer change customer.id customer.id string

### num 10
create view as (select * from billing b left outer join customer c on (b.id = c.id))

### num 11

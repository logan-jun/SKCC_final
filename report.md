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

![Image of map](/hive%20table%20authors%20posts.PNG)







# part 2

3
create table solution as select c.id as id, c.fname as fname, c.lname as lname, c.hphone as hphone from customer c join account a on (c.id = a.custid) where a.amount < 0
![Image of map](/p3-2.PNG)

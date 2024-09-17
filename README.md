# Pharmacy Managment System Using C#
Here 3 types of Users Adminstrator, Customer,Pharmacist. We use MS Sql to manage all the datas here. Here 2 types of users can add or delete options. If someone delete or upadate data it automatically effect the database. For showing the data we use datagridviwe.
Create medic table
create table medic(
id int identity(1,1) primary key,

mid varchar(250) not null,

mname varchar(250) not null,

mnumber varchar(250) not null,

mDate varchar(250) not null,

eDate varchar(250) not null,

quantity bigint not null,

perUnit bigint not null
);



Query for View medicine

select * from medic
select * from medic where mname like '"+txtSearch.Text+"%'
delete from medic where mid = '"+MedicineID+"'



Functionality of view medicine button
Here is the database table

image

When you type medicine name in the search box if the medicine is available then it will automatically show in the datagridview. We can also select any row and delete parmaently using the Delete button. It will automatically delete from the database
image




Query for Add medicine

insert into medic (mid, mname, mnumber, mDate, eDate,quantity, perUnit) values('"+ mid + "','"+ mname + "', '"+ mnumber + "', '"+mdate+"', '"+edate+"',"+quantity+","+perunit+")


Functionality of Add medicine button

Using this we can add new medicine in the database. Here we have to fill all the textbox . We can write the medicine name, medicine ID, quantity, price per unit. After fill all the boxs if we click on add button it will automatically added to the database.

![image](https://github.com/user-attachments/assets/db05f31d-be9a-4577-8387-4ed649562c73)
About
No description, website, or topics provided.
Resources
 Readme
 Activity
Stars
 0 stars
Watchers
 1 watching
Forks
 0 forks
Report repository
Releases
No releases published
Packages
No packages published
Deployments
6
 github-pages 5 days ago
+ 5 deployments
Languages
C#
100.0%
Footer

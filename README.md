# Pharmacy Managment System Using C#
Here 3 types of Users Adminstrator, Customer,Pharmacist. We use MS Sql to manage all the datas here. Here 2 types of users can add or delete options. If someone delete or upadate data it automatically effect the database. For showing the data we use datagridviwe.
#Create medic table
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



# Query for View medicine

select * from medic
select * from medic where mname like '"+txtSearch.Text+"%'
delete from medic where mid = '"+MedicineID+"'



# Functionality of view medicine button
Here is the database table

<img width="828" alt="Screenshot 2024-09-17 at 10 26 45 PM" src="https://github.com/user-attachments/assets/282325a2-ffff-473f-a6bb-ef909ed749aa">


When you type medicine name in the search box if the medicine is available then it will automatically show in the datagridview. We can also select any row and delete parmaently using the Delete button. It will automatically delete from the database
<img width="625" alt="image" src="https://github.com/user-attachments/assets/85fe44f1-2668-484d-ac9a-f95c95477914">





# Query for Add medicine

insert into medic (mid, mname, mnumber, mDate, eDate,quantity, perUnit) values('"+ mid + "','"+ mname + "', '"+ mnumber + "', '"+mdate+"', '"+edate+"',"+quantity+","+perunit+")


# Functionality of Add medicine button

Using this we can add new medicine in the database. Here we have to fill all the textbox . We can write the medicine name, medicine ID, quantity, price per unit. After fill all the boxs if we click on add button it will automatically added to the database.

![image](https://github.com/user-attachments/assets/db05f31d-be9a-4577-8387-4ed649562c73)


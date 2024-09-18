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



# Query for add user

insert into users(userRole,name,dob,mobile,email,username,pass) values ('"+role+"','"+name+ "','"+dob+"',"+mobile+",'"+email+"','"+username+"','"+password+"')![image](https://github.com/user-attachments/assets/a6dec5ac-a739-4bae-b501-851dfd3e75d4)



# Functionality of add user button
Here is the database table

<img width="812" alt="Screenshot 2024-09-18 at 8 45 54 AM" src="https://github.com/user-attachments/assets/b2883307-86c8-4dfc-81ff-fc1fec4ecfb1">



When you type add user name in the search box if the user role then it will automatically show in the datagridview. We can also select any row and delete parmaently using the Delete button. It will automatically delete from the database
<img width="723" alt="Screenshot 2024-09-18 at 8 48 35 AM" src="https://github.com/user-attachments/assets/fef32c5a-a661-4804-930d-35e9233ad911">





# Query for Add user button

insert into medic (mid, mname, mnumber, mDate, eDate,quantity, perUnit) values('"+ mid + "','"+ mname + "', '"+ mnumber + "', '"+mdate+"', '"+edate+"',"+quantity+","+perunit+")


# Functionality of view user button
using this batton show database all user.

<img width="434" alt="Screenshot 2024-09-18 at 8 52 25 AM" src="https://github.com/user-attachments/assets/b0df307c-bc5a-4630-a135-47d53e11608a">


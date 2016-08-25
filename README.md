# MySQL-language
//Steps to start working with MySQL using php devserver   

first when you start to work in php open the php devserver in the computer, click dashboard in the link of the php, then start the apache in http server to run the program, then start the MySQL in database to run the program, then start working with the text editor for instance sublime text and the url where is located the php devserver, it looks like these http://127.0.0.1/ 
Then, look in the dashboard for the name Modules MySQL Administration: PhPMyAdmin click open then, it will go to the page to start working in MySQL this is the url of the page  27.0.0.1/eds-modules/phpmyadmin4551x160814153047/server_databases.php?db=&amp;token=43298883021ef11904743fb426f7828a  

To set up a workplace,   
first need a database, go to database create one name accounts, then, click in account you can see it in the left side, create now a table inside the database account named users specifying how many table do i want to have for each user information. 
I set 5 columns, since i want to each users have a ID, username, password, first name, last name. After that, we write ID, then in type we put INT(means integer=number), then we scroll and look for index and put primary  (what means index primary it will look this value as primary key first access in the table), then A_I click it( what  means A_I stands for auto increment first value we have with increment by one with this, so it will create each user  a unique ID)  

So then, we write Username, then in type we put VARCHAR(we used this since it allows to put a length, since TEXT used  more memory instead, then we are putting a length of 20 characters. 
Then, we write Password, then in type we put VARCHAR(we used this since it allows to put a length, since TEXT used  more memory instead, then we are putting a length of 20 characters.  
Then, we write First, then in type we put VARCHAR(we used this since it allows to put a length, since TEXT used  more memory instead, then we are putting a length of 20 characters.  
Then, we write Last, then in type we put VARCHAR(we used this since it allows to put a length, since TEXT used  more memory instead, then we are putting a length of 20 characters.   

If you miss, or need to add another column go up at the beginning of the table, specify how many column do you want to  have, in here we will type 1 and go.  Then, we write About, then in type we put TEXT(since some person what to write a lot about themself we leave it like  that). Then, click SAVE!  Then, you have create the table. You can see the structure of the table by click in on structure. But since the table doesn't have content, we need to add it. So we click insert.  For the column ID, we leave it blank. 

For the column Username, in value we put TeachMeComputer. 
For the column Password, in the value we put password123. 
For the column First, in value we put Chris. 
For the column Last, in value we put Johnson. 
For the column About, we put we put My name is Chris. 
Then, you go to Go at the end of the file, you will see you create this content is in green.  

Now, how to connect a file from php with MySQL database steps. 

First create a file called mysql.php with sublime text  &lt;

?php  mysqli_connect("localhost", "root","") or die (mysqli_error());  //here the name of the host, username called root, since i don't have a password empty, we set a fucntion or die to make an error if it doesn't connect.   

?>

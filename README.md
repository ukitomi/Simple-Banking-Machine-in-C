# Simple-Banking-Machine-in-C
A program using embedded C and SQL. The user interface has not been develop yet, in order to navigate through the program, please use terminal.

## Getting Started
The readme will include step-by-step instructions on how to run and test the files.

### Prerequisites
* Any text editor. ![I used Sublime Text 3](https://www.sublimetext.com/3)
* Any functional Database (I used [IBM DB2](https://www.ibm.com/analytics/us/en/db2/trials/))![](https://cdn.discordapp.com/attachments/316348168465809408/387138474920378368/unknown.png)

### Installing
#### Step 1. 
Log into your database application. In there, access your database terminal. The command line should be given. ![It looks like this in DB2](https://cdn.discordapp.com/attachments/316348168465809408/387361364622180359/unknown.png)

#### Step 2.
In the terminal, open up the text editor. For me, it's VI text editor. ![Check here for command instructions](https://www.cs.colostate.edu/helpdocs/vi.html)

#### Step 3.
Copy and paste the code in p2.sqc under repository to the text editor in the terminal. Save it as **p2.sqc**

#### Step 4.
In your database application, create an actual database. [It looks like this in IBM DB2](https://cdn.discordapp.com/attachments/316348168465809408/387145801740189696/unknown.png)

#### Step 5.
Copy and paste the file contents under create.txt to your database app. [It looks like this in IBM DB2](https://cdn.discordapp.com/attachments/316348168465809408/387355756099403797/unknown.png)

Those are the create table statements needed in order to test our program.

#### Step 6.
At this point, all the files are ready to go for testing. Tables are included in the database too.

## Running the tests
=> Make sure that the database contain the **tables needed**.

Copy and paste the following lines into the terminal.
```
(Database application name) Connect to <Your database name>
(Database application name) Prep p2.sqc
cc -I./sqllib/include -c p2.c
cc -o p2 p2.o -L./sqllib/lib  -ldb2
./p2 db.properties
```

and the output should look exactly the same like in output.txt file.

To begin testing, simply follow the instructions on the terminal.

## Built with
* embedded C - The program framework
* SQL - Managed data in the database

## Author
* ![Yuki Ou](https://github.com/ukitomi)

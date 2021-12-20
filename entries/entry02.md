# Entry 2
### 12/13/2021

***CONTEXT:***
<br>
For the past month, I have been working with my partner, Sarah, in learning the different parts of [CS50](https://cs50.harvard.edu/college/2021/fall/) that we would be using to create our web application of a study guide. There are four parts that we are focusing on in creating our study guide, [Python](https://cs50.harvard.edu/college/2021/fall/weeks/6/), [SQL](https://cs50.harvard.edu/college/2021/fall/weeks/7/), [HTML, CSS, JavaScript](https://cs50.harvard.edu/college/2021/fall/weeks/8/), and [FLASK](https://cs50.harvard.edu/college/2021/fall/weeks/9/). By working with my partner, we came up with this learning/working system where she would be learning and tinkering with Python while I experiment with SQL and exchange what we have learned with each other. 
_____
***ENGINEERING DESIGN PROCESS:***
<br>
Throughout the Engineering Design Process, I am currently brainstorming possible solutions since there are multiple parts in the web application of a study guide. As I watched and followed along with Professor Malan, I was confused with the concept of Python and SQL. So I did some additional research to better understand what SQL is and its different components. With this, I was able to understand that SQL, Structured Query Language, is a standard language for storing, editing, and adding/deleting data in databases (Python in this case). From [W3Schools](https://www.w3schools.com/sql/default.asp)' SQL Tutorial, I was able to understand that there are two main components in SQL, linking to a database and knowing the syntaxes. I have begun learning some of the syntaxes for SQL and took a sneak-peak of how SQL is linked to a database on W3Schools which then when I rewatched the lecture, I was able to determine where Professor Malan got his code for connecting Python with SQL. SQL linking with Python code from the lecture:

```ruby
 1  import csv 
 2  
 3  from cs50 import SQL
 4  
 5  db = SQL("sqlite:///favorites.db")
 6  
 7  title = input("Title: ").strip()
 8  
 9  rows = db.execute("SELECT COUNT(*) AS counter FROM favorites WHERE title LIKE ?", title)
10 
11  row = rows[0]
12
13  print(row["counter"])
```
Line 1 gets data from CSV (Comma Separated Values library). Line 3 imports SQL so that it can be linked with Python. Line 5 creates a variable called db (database) and opens up the database. Line 7 creates a variable called title where it asks the user for a title while removing any whitespace with `.strip()`. Line 9 returns a list (rows) where `.execute()` takes in SQL command from the original Python. The SQL keyword `SELECT` is used to select data from a database where the data returned is stored in a result table. The SQL `*` is used to specify that the query should return all columns of the queried tables. The SQL keyword `WHERE` is used to filter records and extract records that fulfill a specified condition only. Line 11 grabs the first row from the rows that were executed. Line 13 prints out the row's first value.
_____
***SKILLS:***
<br>
The skills I used are **Collaboration** and **Communication**. The skill **Collaboration** allowed me and my partner to split the learning process making it easier to understand the concept we are focusing on. As a result, each of us can focus on a specific part to learn without worrying about the other parts. **Communication** is a skill that I continued using because each of us is learning different parts in constructing the web application, so I need to communicate with my partner about what I've learned and vice versa in addition to making everything organized. By doing this, each of us would have an idea of what each part is talking about.

[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)

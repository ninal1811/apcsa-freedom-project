# Entry 4
### 3/14/2022

***CONTEXT:***
<br>
Throughout the past week, I focused on starting the MVP (the core base of the project). My partner and I worked together in learning more about Flask and how we can incorprate it into our project. 
_____
***ENGINEERING DESIGN PROCESS:***
<br>
Throughout the Engineering Design Process, I am currently in **Creating the Prototype**. Since I've learned my tool, I've began implamenting what I've learn into my project in creating a **Study Guide for the APCSA Exam**. According to our MVP Plan, I foucused mainly on the HTML file. In deciding our project's basic layout, I took considerate of [W3Schools](https://www.w3schools.com/java/default.asp) and [Gmail](https://www.gmail.com). From these websites, I've realized that the navageation bar are mainly located on the left side of the screen where users are able to have the majority of the right space to look at content. By putting the navagation bar on the left side, it allows users to have easy access to all the units without filling up too much of the space for content. Below is our basic start for our project:

![276000138_751626785822240_8828296280061258519_n](https://user-images.githubusercontent.com/56265101/159405284-2feeadb2-fff9-4cd4-ae7f-923250c9db1f.png)

We decided to use Flask because it allows use to import libraries that we can use for our project. But, as of right now, Flask is being used as a small "function" where is allows us to link the different units onto one base file. 

```java
from flask import Flask,render_template,request

app = Flask(__name__)

@app.route("/")
def index():
  return render_template("index.html")
```

From the basic `app.py` template of Flask, my partner (Sarah) has modtified this code where it is unique for our project. 

```java
from flask import Flask

app = Flask(__name__)

from app import routes
```

By adding `from app import routes`, it personializes the Flask to link towards the routes of where we would be requesting the web browser for which the routers are linked to. Adding on, `@app.route` allows the files to be accessed through the URL which results a platform where we are able to link our files. 

```java
from flask import render_template
from app import app

@app.route('/')
@app.route('/home')
def home():
    return render_template('home.html')
```

From the HTML file presented in the last blog entry, my partner and I have modtifyed it as we worked on impleamenting Flask into our project.

```html
...
</style>   
    </head>

    <body>
        <div class="sidebar">
            <div><a href = "/home">Home</a></div>
            <div><a href = "/unit1">Unit 1: Primitive Types</a></div>
            <div><a href = "/unit2">Unit 2: Using Objects</a></div>
            <div><a href = "/unit3">Unit 3: Boolean Expressions / If statements</a></div>
            <div><a href = "/unit4">Unit 4: Iteration</a></div>
            <div><a href = "/unit5">Unit 5: Writing Classes</a></div>
            <div><a href = "/unit6">Unit 6: Array</a></div>
            <div><a href = "/unit7">Unit 7: ArrayList</a></div>
            <div><a href = "/unit8">Unit 8: 2D Array</a></div>
            <div><a href = "/unit9">Unit 9: Inheritance</a></div>
            <div><a href = "/unit10">Unit 10: Recursion</a></div>
        </div>
       <div class ="content">
           {% block content %}{% endblock %}
       </div>

    </body>
</html>
```
The code above presents the navagation bar for which users are able to use in navigating to different content. `{% block content %}{% endblock %}` defines where derived templates are able to insert themselves. Since `blocks` is a unquie name, it is able to reference the templates when content is being provided. 

_____
***SKILLS:***
<br>
The skills I used are paying **Attention to Details** and **Consideration**. The skill **Consideration** allows me to be considerate of how others can use and navigate through the website. For instance, considering with a side navagation bar allow it to be more benefitcal in using because it would be difficult for people to determine which unit they are currently in. Paying **Attention to Details** is another skill that I have learned throughout tinkering and building a base for my application. Since I am working with a partner, we are able to catch the small details that could possibliy be disrupting our program. 

_____
***NEXT STEP:***
<br>
My next steps would be spliting the content work with my partner where we add contents from each unit. As we progresses through the contents, we will make further adjustment towards the layout and including other features such as quizzes. 

[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)

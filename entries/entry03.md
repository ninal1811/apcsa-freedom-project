# Entry 3
### 2/7/2022

***CONTEXT:***
<br>
For the past weeks, I have been working on learning my tool, [CS50](https://cs50.harvard.edu/college/2021/fall/). Sarah and I have planned to create a study guide for the APCSA exam using what we have learned from CS50. As Sarah is focusing on learning [Flask](https://cs50.harvard.edu/college/2021/fall/weeks/9/), I have started to create a layout for our application. 
_____
***ENGINEERING DESIGN PROCESS:***
<br>
Throughout the Engineering Design Process, I am currently in between **Plan the most promising solution** and **Create a prototype**. Since my partner and I have begun discussing how we want our applications to look, I took Sarah's idea of building a base template then including add-ons of other features. The product we had in mind was that there would have a front page where it contains the overview of the APCSA course and there would have a side/top bar holding each unit/topic where users can interact with it, in addition, to view certain topics in the course. Thus, I have started my HTML page with the initial setup of having the `head`, `body`, and linking `CSS` and `JavaScript`. Below, I have the basic outline of our application that is shown in the HTML file:

```html
<!DOCTYPE html>
<html lang="en">
    
    <head>
        <link rel="stylesheet" href="../style.css" type="text/css">
    </head>
    
    <body>
        <div class="course">
            <h1>APCSA</h1>
            <p>[Insert course overview]</p>
        </div>
      
        <div class="units">
            <div class="leftcolumn">
                <div class="card">
                    <a class="text_size" href="../units/unit_1.html">Unit 1</a>
                    <a class="text_size" href="../units/unit_2.html">Unit 2</a>
                    <a class="text_size" href="../units/unit_3.html">Unit 3</a>
                    <a class="text_size" href="../units/unit_4.html">Unit 4</a>
                    <a class="text_size" href="../units/unit_5.html">Unit 5</a>
                    <a class="text_size" href="../units/unit_6.html">Unit 6</a>
                    <a class="text_size" href="../units/unit_7.html">Unit 7</a>
                </div>
            </div>
        </div>
      
        <script src="../script.js"></script>
    </body>
  
</html>
```
As of right now, the class `course`, presents a header where information about APCSA could be presented. The class `units` is currently a horizontal bar where users can click on each unit and it takes them to a new page. As my partner and I work on adding content to each page, each unit has an interactive link that takes to that unit/topic they want to learn/review. Below is what I have in my CSS file:

```css
body {
    background: #f1f1f1;
}

.course {
  padding: 5px;
  text-align: center;
  background: white;
}

.text_size {
    font-size: 20px;
}

.leftcolumn {
  float: left;
}

.card {
  background-color: white;
  padding: 20px;
  margin-top: 20px;
}
```
When I was adding the columns to my project page, I realized that there isn't a color difference between the body and the column itself. Therefore, I incorporated some color code in the CSS file to better distinguish the columns. 

After conversing with my partner about Flask, I've learned that Flask is a micro web framework written in Python. The basic `app.py` templet is below:
``` python 
1 from flask import Flask, render_template, request
2 
3 app = Flask(__name__)
4 
5 
6 @app.route("/")
7 def index():
8     return render_template("index.html")
```
Line 1 imports Flask from the flask libraries. `app` in line 3 is the file name which is also the flask variable name. Line 6 is a function that labels for the `/` route where `@app.route` is from Flask and the `@` modifies the function. Line 7 is a function that with render the template from the index.html file.
_____
***SKILLS:***
<br>
The skills I used are **Organization** and **Consideration**. The skill **Consideration** allows me to be considerate of how others can use and navigate through the website. For instance, if I didn't make the units show up on the side/top of the application, it would be difficult for people to determine which unit they are currently in. **Organization** is another skill that I have learned throughout tinkering and building a base for my application. Since my partner and I are planning to create a study guide, I believe that it is important to keep everything organized as each unit presents a different topic in the course of APCSA. 

_____
***NEXT STEP:***
<br>
Since I have worked on creating a based template of our project. I believe the next steps are to communicate with my partner about adding information and tweaking the base template of what I have created. By creating an MVP or Minimum Viable Product for our project, Sarah and I would have a project where it is beneficial for others as well as ourselves. I believe this is more important than focusing on the style because having an MVP can present units/topics within the course compared to having a project that doesn't present any information but style.

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)

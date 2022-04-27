# Entry 5
### 04/25/2022

***CONTEXT:***
<br>
Throughout the past weeks, I have been finishing my MVP by importing all the keynotes and ideas for the APCSA course. As we decided to use CS50 as our tool, we are mainly focusing on Python and Flask.

_____
***ENGINEERING DESIGN PROCESS:***
<br>
Throughout the Engineering Design Process, I am currently **Test and evaluating the prototype**. Since we added all the content of Unit 1 - 10, we are done with the webpage information-wise. This leaves me and my partner to focus on the adjustments that need to be made in order to make our webpage more beneficial and efficient to use. As a result, I would also say that based on the Engineering Design Process, we are **Improving as needed**. With the basic layout of the base page, I am planning to implement the same layout for the other pages of the application. 

![276000138_751626785822240_8828296280061258519_n](https://user-images.githubusercontent.com/56265101/159405284-2feeadb2-fff9-4cd4-ae7f-923250c9db1f.png)
As I was adding content to each unit, I ended up with the units that looked like the [page layout example](https://mail-attachment.googleusercontent.com/attachment/u/1/?ui=2&ik=cddeae6d64&attid=0.12&permmsgid=msg-f:1731039842112402608&th=1805e390a12874b0&view=att&disp=inline&realattid=f_l2e0cix111&ser=1&saddbat=ANGjdJ_VCa7oEHjll14CyjjbqSwke1fRsCsRf85cEyKigWdlUpMFXizsrSWBzHgzf3Azi2gJX1FCVkDnKvEn9GSPSIV3DYHjv2lMK7NAfQc0aOKwQnqigCsp2EeLT37Kg06UCxjVtwHzApBBzUOaF4XnRIlUeyVzEaEhBBWIlnjgH58ktk6jS7reYdDfWmgtbgBfH6uCkBj977wx1X4jXJp1PabHx9iio1vn_K6cHSmAalvnhUVYRAauxfOzBw51aaeMinxnc-zpZjedUH2Zuw49JvMSU8obXe-kH7WedtFO0RBubZsbNP_Z_dqN4VaCESAf57d3C_mfH0poBo5gOG4hO7Xoj9NYma_BWwMNv_zFZpl12q0BPsFXJkLJbU-lwOWZYp0EAtRKLU3ISfXU0Qhm54siTjJSIfQXlBcZy3v9MgsWIp3xa37c0zE_EFjl0969TyMSRnwI2NRV9i2uGS3Z7XI_3ONNLWHG8MYLDV4yYkqrHbDpZBZ8QThr3WyxprCZ2W4QWJMYhWttJDKBrj2HcKyuTrU8CExvKC6PKzcwIN4TTwSZnYh5Vlx7YKzjPem8yWbbhZ5_WRtPqu0tLbvTBZWhjswVi5uZrzG3LsHug994K9VzG-I9mnSDNGeMpkLFdDmCAzCT-aOQVuvtRRQPsYKK4KiCBNuRgwZXWTF7v4X7Xle0B_GML7w63frcNfGulLiD07UOnc44dfj_BaD0f3OiNNgjeYPRaZkely-uEDuA6bTiVWpMkgWLyhDHE6ZPRmc-NaEorxi6oG9WcMvGJicVI0tdGibJq5QjFhbNNzpVyMPHMvL6zaqktAbtLsq-hlfMVinwLBqdkuHh). Thus, I am working with my partner in debugging and deploying the code so that users would be able to navigate within the pages of the units making it more efficient to use. 

```html
<html lang="en">
  <head>
    ... 
  </head>
  {% extends "base.html" %}

  {% block content %}
    <h1>Unit 7: ArrayList</h1>
      <div class = "part1">
        <h4>What are Arraylists?</h4>
        <body>An ArrayList is a collection or list that <i>only</i>stores class data types, or objects. It is similar to a regular array, but it’s really only storing references to the data it contains. The size of arraylist is not fixed which means that adding or removing elements in an arrayList will not lose data. To  declare ArrayList use <code>ArrayList<DataType> list = new ArrayList<DataType>();</code>. Like arrays, arraylists has index and starts at 0 too. Standards numbers which are stored in primitive cannot be added to an ArrayList but we do have wrapper classes and we can use unboxing and autoboxing to address this issue. Built-in methods that arraylist provided:
         ...
         </body>
        
   {% endblock %}
</html>
```
The code above presents the basic structure of how information on each unit is being placed, but there isn't a navigation bar within the units to allow easy access to other units. Hence, we need to debug/add the navigation bar and adjust the layout of our webpage.

_____
***SKILLS:***
<br>
The skills I used are **Consideration** and **Embracing failure**. As this webpage is meant to benefit others in knowing and understanding the concepts of APCSA, we took into consideration how we would like to layout the information presented as the order of how we would input pieces of information. Embracing failures is another skill I've used because learning a tool may seem easy, but reflecting on what I have learned on a webpage may be annoying and difficult. Thus, embracing my failures would allow me to grow and understand the key points that I might have missed.

_____
***NEXT STEP:***
<br>
My next steps would be debugging to ensure that the webpage runs smoothly without errors. After that, we would be working on the layout and make further adjustments if needed. 

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)

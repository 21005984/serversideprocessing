# Design a Website for Server Side Processing

## AIM:
To design a website to perform mathematical calculations in server side.

## DESIGN STEPS:

Step 1:
Desing your website for calculation using wireframe work.

Step 2:
Then to execute the wireframe work desing use html,css

Step 3:
Use views.py to execute the coding in serverside.

Step 4:
Mention the path of the website in urls.py.

Step 5:

Publish the website in the given URL.: http://meiyarasi.student.saveetha.in/

## PROGRAM :
<!DOCTYPE html>
<html>
<head>
    <meta charset='utf-8'>
    <meta http-equiv='X-UA-Compatible' content='IE=edge'>
    <title>Math Calculation</title>
    <meta name='viewport' content='width=device-width, initial-scale=1'>
    <script src='main.js'></script>
    <style>
        * {
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
body {
  background-image: url("/static/img/m.jpg");
}
.container {
  width: 1080px;
  margin-left: auto;
  margin-right: auto;
  padding-top: 200px;
  padding-left: 300px;
}
.content {
  display:block;
  width: 500px;
  min-height: 300px;
  font-size: 20px;
  background-color:white;
}
h1{
    color: blue;
    text-align: center;
    padding-top: 25px;
}
.formelement{
    color: blue;
    text-align: center;
    margin-top: 5px;
    margin-bottom: 5px;
}
    </style>
</head>
<body>
    <div class="container">
    <div class="content">
    <h1>VOLUME OF A CUBOID</h1>
    <form method="POST">
        {% csrf_token %}
        <div class="formelement">
        Length : <input type="text" name="length" value="{{l}}"></input>Meters<br/>
        </div>
        <div class="formelement">
        Breadth : <input type="text" name="breadth" value="{{b}}"></input>Meters<br/>
        </div>
        <div class="formelement">
        Width : <input type="text" name="width" value="{{w}}"></input>Meters<br/>
        </div>
        <div class="formelement">
        <input type="submit"  value="Calculate Volume"></input><br/>
        </div>
        <div class="formelement">
        Volume : <input type="text" name="volume" value="{{volume}}"></input>Meter<sup>3</sup><br/>
        </div>
    
    </form>
    </div>
    </div>
</body>
</html>


## OUTPUT:

### Home Page:
![Screenshot (103)](https://user-images.githubusercontent.com/94748389/155069921-afb09253-d46c-412d-bf26-e29c84970d04.png)


## Result:
Thus a website is designed to perform mathematical calculations in server side and is hosted at http://meiyarasi.student.saveetha.in/

# Web Page for Mathematical Calculations
## AIM:
To design a static website with validation to perform mathematical calculations in client side.
## DESIGN STEPS:
### Step 1:
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Write javascript to perform the calculations.
### Step 4:
Include regularexpression based input validation.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.
## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Volume</title>
    <style>
        * {
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
body {
  background-color:rgb(125, 125, 145);
}
.container {
  width: 1080px;
  margin-left: auto;
  margin-right: auto;
}
.content {
  display: block;
  width: 100%;
  background-color:green;
  min-height: 500px;
  margin-top: 150px;
}
.content2{
    display: block;
    width: 100%;
    background-color:blue;
    min-height: 500px;
    margin-top: 150px;
    margin-bottom: 150px;
}
h1{
    text-align: center;
    padding-top: 50px;
    color: rgb(36, 23, 23);
}
.formelement{
    text-align: center;
    font-size:xx-large;
    margin-top: 5px;
    margin-bottom: 5px;

}
    </style>
</head>
<body>
    <div class="container">
        <div class="content">
            <h1>VOLUME OF CYLINDER</h1>
            <form>
                <div class=formelement>
                    <lable for="aedit">Height:</lable>
                    <input type="number" id="aedit" value="0"/>
                </div><br>
                <div class=formelement>
                    <lable for="bedit">Radius:</lable>
                    <input type="number" id="bedit" value="0"/>
                </div><br>
                <div class=formelement>
                    <input type="button" value="CALCULATE" id="calbutton"/>
                </div><br>
                <div class=formelement>
                    <lable for="cedit">Volume:</lable>
                    <input type="text" id="cedit" readonly="0"/>
                </div><br>
                <div class=formelement>
                    Formula is = pi*Radius^2*Height
                </div>
            </form>
        </div>
        <script type="text/javascript">
            var button;
            button=document.querySelector("#calbutton");
            button.addEventListener("click",function(){
                var anumber,bnumber,cnumber;
                var aval,bval,cval;
                anumber=document.querySelector("#aedit");
                bnumber=document.querySelector("#bedit");
                cnumber=document.querySelector("#cedit");

                aval=parseInt(anumber.value);
                bval=parseInt(bnumber.value);
                cval=(22/7)*aval**2*(bval);
                cnumber.value=""+cval;
            });
        </script>
        <div class="content2">
            <h1>VOLUME OF CONE</h1>
            <form>
                <div class="formelement">
                  <lable for="radiusedit">RADIUS:</lable>
                  <input type="text" id="radiusedit" value=" "/>
                </div><br>
                <div class="formelement">
                  <lable for="heightedit">HEIGHT:</lable>
                  <input type="text" id="heightedit" value=" "/>
                </div><br>
                <div class="formelement">
                  <input type="button" value="CALCULATE" id="calbutton"/>
                </div><br>
                <div class="formelement">
                  <lable for="volumeedit">VOLUME:</lable>
                  <input type="text" id="volumeedit" readonly="0"/>
                </div><br>
                <div class="formelement">
                Formula is:V=π*Radius^2*Height/3
                </div><br>
                
            </form>
    
            </div>
        </div>
        <script type="text/javascript">
          var button;
          button=document.querySelector("#calbutton");
          button.addEventListener("click",function(){
            
              var radiustext,heighttext,volumetext;
              var aval,bval,cval;
    
              radiustext=document.querySelector("#radiusedit");
              heighttext=document.querySelector("#heightedit");
              volumetext=document.querySelector("#volumeedit");
      
              aval=parseInt(radiustext.value);
              bval=parseInt(heighttext.value);
              cval=(22/7)*(aval**2)*(bval/3);
              volumetext.value=""+cval;
        
      
            });
      
        </script>     
<footer>By Sai Darshan</footer>
</body>
</html>
```
## OUTPUT:
![GitHub Logo](3.png)

## Result:
Thus a website is designed to perform mathematical calculations in the client side.

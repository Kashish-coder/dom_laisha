# dom_laisha
```!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
    <h2>Javascript can change html</h2>
    <p id="p1">Hello world</p>
    <script>
        document.getElementById('p1').innerHTML="New paragraph text generated";
    </script>
    <p>Above para is  changed</p>
    
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h2>
        JS htnl dom
    </h2>
    <p>Finding html elements using object</p><br>
    <form id="form" action="/action-page.php">
        first name:<input type="text" name=fname
 value="Donald"><br>
 last name:<input type="text" name=lname
 value="Duck"><br>
 <input type="submit" value="submit">
    </form>
    <p>Here are values of each element</p>
<p id="demo">
</p>
<script>
    const x=document.forms["form"];
    let text="";
    for(let i=0;i<x.length;i++){
    text+=x.elements[i].value +"<br>";}

document.getElementById("demo").innerHTML=text;
</script></body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
.demo{
    color:red;}
    </style>
<body>
    <h1 id="h1">The element object</h1>
    <h2>The setattribute method</h2>
    <p>Click add class to add a class attribure to h1 element</p>
   <button onclick="myfunction()">Add class</button>
</body>
<script>
    document.write(Date());
    function myfunction(){
        document.getElementById("h1").setAttribute("class","demo");
    }
</script>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <img id="img" src="https://media.gettyimages.com/id/1744858552/photo/carnaby-street-london-uk.jpg?s=612x612&w=gi&k=20&c=xrbvT0gXswU-aa5Wl-kW28D-SP22vdINsgOoZf2GuoA=" width="160" height="120">
    <script>
        document.getElementById('img').src="https://media.gettyimages.com/id/2149820887/photo/abstract-landscape-background.jpg?s=612x612&w=gi&k=20&c=WSOm8eLitpSfSSwU7a6DfBs6Hd2jwT11ote_zAhKHSQ="
    </script>
</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>The document object</h1>
    <h2>create ele method</h2>

    <p>Create ele and append it to "myDiv"</p>
    <div id="myDiv" style="padding:16px;
    background-color: pink;">
    <h3>A div element</h3>
</div>
    <script>
        const para=document.createElement("p");
        para.innerHTML="this is a para";
        document.getElementById("mydiv").appendChild(para);
    </script>
</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        .bg-black{
            background-color: aqua;
            color:aliceblue

        }
    </style>
</head>
<body>
    <form id="form" action="/action_page.php">
        first name:<input type="text" name=fname
 value="Donald"><br>
 last name:<input type="text" name=lname
 value="Duck"><br>
 <input type="submit" value="submit">

    </form>
    <p>click try it button to display number of elements in form</p>
    <button onclick="myfunction()">Try it</button>
    <p id="displayspace"></p>
    <script>
        function myfunction(){
            var x=document.getElementById("form").elements.length;
            var y=document.getElementById("form").elements[0].value;
            document.getElementById("displayspace").innerHTML="found"+x+" elements in form"+" first name entered is "+y;
        


        //create element and insert in dom 
        const para=document.createElement("p");
        para.innerText="This is a para created via dom";
        document.body.appendchild(para);}
    </script>
</body>
</html>```
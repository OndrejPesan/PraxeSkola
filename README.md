# PraxeSkola
práce ve škole a školní projekty na hodinách PRX
HTML:
<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" type="text/css" href="1prx.css" />
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> How to calculate that </title>
    <script src="1prx.js"></script>
</head>
<body>
    <header>
    <h1><b>Volume & Surface Area in Math</b></h1>
    </header>
    <div class="txt">
    <p>If you have problem with those two. Don't worry, Ferdinand will help you, how to calculate that.</p>
    <p2>He's programmed to calculate these. In no time you'll have correct awnsers.</p2>
    </div>
    <div class = "boxes">
        <div class = "leftbox">
            <h2>Cube</h2>
           <div>
            <p>Cube Surface Area can be count like that:</p>
            6*a*a
            <p>and Volume just like that:</p>
            a*a*a or a3
            <input type="text" id="numInputA" placeholder="Enter edge (a)">
            <button>Calculate</button>
            <script>
                function result() { var numberA = document.getElementById("numInputA").value;
                   if (!isNaN(numberA))
                      console.log("The value=" + parseInt(numberA));
                   else
                      console.log("Please enter the integer value..");
                }
             </script>
           </div>
        </div>
         
        <div class = "middlebox">
            <h2>Cuboid</h2>
            <div>
                <p>Cuboid Surface Area can be count like that:</p>
                2*(a*b+a*c+b*c)
                <p>and Volume just like that:</p>
                a*b*c
                <input type="text" id="numInputX" placeholder="Enter 1st dimension (x)">
                <input type="text" id="numInputY" placeholder="Enter 2nd dimension (y)">
                <input type="text" id="numInputZ" placeholder="Enter 3rd dimension (z)">
                <script>
                    function result() { var numberX = document.getElementById("numInputX").value;
                       if (!isNaN(numberX))
                          console.log("The value=" + parseInt(numberX));
                       else
                          console.log("Please enter the integer value..");
                    }
                    function result() { var numberY = document.getElementById("numInputY").value;
                       if (!isNaN(numberY))
                          console.log("The value=" + parseInt(numberY));
                       else
                          console.log("Please enter the integer value..");
                    }
                    function result() { var numberZ = document.getElementById("numInputZ").value;
                       if (!isNaN(numberZ))
                          console.log("The value=" + parseInt(numberZ));
                       else
                          console.log("Please enter the integer value..");
                    }
                 </script>
                <button data-calc>Calculate</button>
               </div>
        </div>
         
        <div class = "rightbox">
            <h2>Cylinder</h2>
            <div>
                <p>Cylinder Surface Area can be count like that:</p>
                2*pi*r*h+r*r*pi or 2*pi*r*h+r2*pi
                <p>and Volume just like that:</p>
                r*r*h*pi or r2*h*pi
                <input type="text" id="numInputR" placeholder="Enter radius (r)">
                <input type="text" id="numInputH" placeholder="Enter high (h)">
                <button>Calculate</button>
                <script>
                    function result() { var numberR = document.getElementById("numInputR").value;
                       if (!isNaN(numberR))
                          console.log("The value=" + parseInt(numberR));
                       else
                          console.log("Please enter the integer value..");
                    }
                    function result() { var numberH = document.getElementById("numInputH").value;
                       if (!isNaN(numberH))
                          console.log("The value=" + parseInt(numberH));
                       else
                          console.log("Please enter the integer value..");
                    }
                 </script>
               </div>
        </div>
    </div>
</body>
</html>
CSS:
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}
body {
    background-color: rgb(55, 64, 70);
    color: rgb(231, 231, 231);  
}
.header {
    width: 100%;
    height: 100vh;
    background: rgb(73, 27, 67);
    
}
.boxes{
    padding: 15px;
}
.leftbox {
    float:left;
    background:Red;
    width:33.333%;
    height:280px;
}
.middlebox{
    float:left;
    background:Green;
    width:33.333%;
    height:280px;
}
.rightbox{
    float:left;
    background:blue;
    width:33.333%;
    height:280px;
}
.txt{
    text-align: center;
}
h1{
    color:rgb(115, 143, 115);
    text-align:center;
}
JS:
var episode = ("V is equal to ")
var serial = ("S is equal to ")

var r = numberR
var v = numberH
var p = 3.14
d = r*r*v*p
console.log(episode+d+"cm3")
o = 2*p*r*v+r*r*p
console.log(serial+o+"cm2")

const calcButton = document.querySelector("[data-calc]")
var t = numberA
pudin=t*t*t
console.log(episode+pudin+"cm3")
e=6*t*t
console.log(serial+e+"cm2")

calcButton.addEventListener("click", () => {
    var rare = numberZ
var common = numberY
var epic = numberX
legendary = rare*common*epic
console.log(episode+legendary+"cm3")
awesome = 2*(rare*common + rare*epic + epic*common)
console.log(serial+awesome+"cm2")
return
    
})

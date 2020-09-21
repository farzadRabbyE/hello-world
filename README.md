<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>Page Title</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
</head>
<body>
    <img id="image" src="of.png" alt="off" />
    <button onclick="lightOn()" >on</button>
    <button onclick="lightOff()">off</button>
    <button id="OnOffButton" onclick="lightOnOff()">OnOff</button>
    <script>
        function lightOn() {
            document.getElementById("image").setAttribute("src","on.png");
        }
        function lightOff() {
            document.getElementById("image").setAttribute("src","of.png");
        
        }
        function lightOnOff() { 
            var imgSrc = document.getElementById("image").getAttribute("src")

            if(imgSrc == "of.png"){
                document.getElementById("image").setAttribute("src","on.png");
                document.getElementById("OnOffButton").innerHTML="off"
            }
            else {
                document.getElementById("image").setAttribute("src","of.png");
                document.getElementById("OnOffButton").innerHTML="on" 
            }
            

        }
    </script>
</body>
</html>

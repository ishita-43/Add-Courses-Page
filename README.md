# NewRepo
#light bulb in working 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Switch Bulb</title>
    <style>
    .center{
        display: block;
        margin-left: auto;
        margin-right: auto;
        max-width: 50%;
        }

    .btn{
        padding: 20px;
        background-color: rgb(3, 94, 3);
        max-width: 100px; 
        }
    </style>
</head>
<body style="background-color:black">
    <img id="bulb" src="img/bulb_off.png" alt="" class="center">
    <button id="togglebtn" class="center btn">Turn On</button>
    <script>
        let btn = document.getElementById('togglebtn')
        let bulb = document.getElementById('bulb')
        btn.addEventListener('click',toggleBulb)
     function toggleBulb(e){
         if(btn.textContent.includes('On')){
         bulb.src = "img/bulb_on.png"
         btn.textContent ="Turn Off"
         }
     else{
         bulb.src = "img/bulb_off.png"
         btn.textContent ="Turn On"
         }
            // console.log(e)
        }
    </script>
</body>
</html>

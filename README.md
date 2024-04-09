<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Just For Fun Devi Ji !</title>
<style>
    .box{
    	margin-top: 150px;
    	margin-left: 60px;
	}
	#yes{
    	border: none;
    	width: 90px;
    	background-color: rgba(33, 240, 105, 0.954);
    	border-radius: 10px;
    	font-size: 25px;
    	padding: 8px;
	}

	#game-container {
    	position: relative;
    	width: 500px;
    	height: 600px;
    	border: 2px solid #333;
    	margin: 5px;
    	overflow: hidden;
        background-image: url(Cartoon4.jpg);
		background-size:contain;
		
	}
	
     #name {
		color: rgb(0, 0, 0);
		padding-top: 10px;
		
		
		
	 }


    h4 {
        font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        color: #000000;
        text-shadow: #333;
		

        
    }
	#target {
    	position: absolute;
    	left: 200px;
    	background-color: #fff200;
    	border: none;
    	width: 90px;
    	border-radius: 10px;
    	font-size: 25px;
    	padding: 8px;
    	cursor: pointer;
    	transition: top 0.5s, left 0.5s;
		
	}
  

</style>
</head>
<body>

<div id="game-container">
	<div class="box">
	<h1 id="name">Do you love me?💓</h1>
	<button id="target">No!</button>
	<button id="yes" >Yes!</button>
	<h4>NO PAR CLICK KARNE KI GALTI MATT KARNA WARNA GARBAR HO JAAYE GA </h4>

 </div>
</div>


<script>
const target = document.getElementById('target');
function moveTarget() {
	const maxWidth =400;
	const maxHeight = 400;

	const randomX = Math.floor(Math.random() * maxWidth);
	const randomY = Math.floor(Math.random() * maxHeight);

	target.style.left = randomX + 'px';
	target.style.top = randomY + 'px';
	}

	target.addEventListener('mouseenter', function() {
    	moveTarget();
	
	
	
	});
</script>

</body>
</html>


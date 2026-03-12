<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Smart Watch Offer</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial;
}

body{
background:#f4f6fb;
}

header{
background:linear-gradient(90deg,#007bff,#00c6ff);
color:white;
padding:25px;
text-align:center;
}

.timer{
background:#ff3b3b;
color:white;
text-align:center;
padding:10px;
font-size:18px;
}

.container{
width:90%;
max-width:1100px;
margin:auto;
margin-top:40px;
display:flex;
flex-wrap:wrap;
gap:40px;
align-items:center;
}

.slider img{
width:100%;
max-width:400px;
border-radius:10px;
}

.details{
flex:1;
}

.price{
font-size:32px;
color:#ff3b3b;
margin:15px 0;
}

.old{
text-decoration:line-through;
color:gray;
margin-left:10px;
}

button{
padding:12px 25px;
border:none;
background:#007bff;
color:white;
font-size:18px;
border-radius:6px;
cursor:pointer;
margin-top:10px;
}

.whatsapp{
background:#25D366;
margin-left:10px;
}

.features{
margin-top:20px;
}

.features li{
margin:8px 0;
}

.reviews{
margin-top:60px;
text-align:center;
}

.review-box{
background:white;
padding:20px;
margin:15px;
display:inline-block;
width:250px;
border-radius:8px;
box-shadow:0 5px 15px rgba(0,0,0,0.1);
}

footer{
margin-top:60px;
background:#222;
color:white;
text-align:center;
padding:20px;
}

@media(max-width:768px){
.container{
flex-direction:column;
text-align:center;
}
}

</style>
</head>

<body>

<header>
<h1>🔥 Smart Watch Mega Offer 🔥</h1>
<p>Limited Stock Available</p>
</header>

<div class="timer">
Offer Ends In: <span id="countdown"></span>
</div>

<div class="container">

<div class="slider">
<img src="product.jpg">
</div>

<div class="details">

<h2>Premium Smart Watch</h2>

<p>Track fitness, heart rate, and daily activity with this stylish smart watch.</p>

<div class="price">
Rs 1999 <span class="old">Rs 3999</span>
</div>

<ul class="features">
<li>✔ Waterproof</li>
<li>✔ Heart Rate Monitor</li>
<li>✔ 7 Day Battery</li>
<li>✔ Fitness Tracking</li>
</ul>

<a href="order.html">
<button>Order Now</button>
</a>

<a href="https://wa.me/923000000000">
<button class="whatsapp">WhatsApp Order</button>
</a>

</div>

</div>

<div class="reviews">

<h2>Customer Reviews ⭐</h2>

<div class="review-box">
⭐⭐⭐⭐⭐  
"Very good quality watch!"
<br>— Ali
</div>

<div class="review-box">
⭐⭐⭐⭐⭐  
"Battery life is amazing."
<br>— Ahmed
</div>

<div class="review-box">
⭐⭐⭐⭐  
"Fast delivery and nice product."
<br>— Sara
</div>

</div>

<footer>
© 2026 Your Brand
</footer>

<script>

var countDownDate = new Date().getTime() + 86400000;

var x = setInterval(function() {

var now = new Date().getTime();

var distance = countDownDate - now;

var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));

var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));

var seconds = Math.floor((distance % (1000 * 60)) / 1000);

document.getElementById("countdown").innerHTML =
hours + "h " + minutes + "m " + seconds + "s ";

if (distance < 0) {
clearInterval(x);
document.getElementById("countdown").innerHTML = "EXPIRED";
}

}, 1000);

</script>

</body>
</html><!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Order Now</title>

<style>

body{
font-family:Arial;
background:#f4f6fb;
}

.container{
max-width:450px;
margin:auto;
margin-top:70px;
background:white;
padding:30px;
border-radius:10px;
box-shadow:0 10px 25px rgba(0,0,0,0.1);
}

h2{
text-align:center;
margin-bottom:20px;
}

input,textarea{
width:100%;
padding:12px;
margin:10px 0;
border:1px solid #ccc;
border-radius:5px;
}

button{
width:100%;
padding:12px;
background:#007bff;
color:white;
border:none;
font-size:18px;
border-radius:6px;
cursor:pointer;
}

button:hover{
background:#0056b3;
}

</style>
</head>

<body>

<div class="container">

<h2>Place Your Order</h2>

<form onsubmit="sendWhatsApp(); return false;">

<input id="name" type="text" placeholder="Full Name" required>

<input id="phone" type="text" placeholder="Phone Number" required>

<textarea id="address" placeholder="Full Address"></textarea>

<input id="qty" type="number" placeholder="Quantity">

<button type="submit">Submit Order</button>

</form>

</div>

<script>

function sendWhatsApp(){

var name=document.getElementById("name").value;
var phone=document.getElementById("phone").value;
var address=document.getElementById("address").value;
var qty=document.getElementById("qty").value;

var message="New Order:%0AName: "+name+
"%0APhone: "+phone+
"%0AAddress: "+address+
"%0AQuantity: "+qty;

window.open("https://wa.me/923000000000?text="+message);

}

</script>

</body>
</html>

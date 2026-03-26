 <html>
<head>
<title>Secret Surprise</title>

<style>
body{
font-family: Arial;
background: linear-gradient(to right,#ffd6e0,#fff0f5);
display:flex;
justify-content:center;
align-items:center;
height:100vh;
text-align:center;
}

.box{
background:white;
padding:40px;
border-radius:15px;
box-shadow:0 0 20px rgba(0,0,0,0.1);
}

input{
padding:10px;
margin-top:10px;
border-radius:8px;
border:1px solid gray;
}

button{
padding:10px 20px;
margin-top:15px;
border:none;
background:#ff4d6d;
color:white;
border-radius:8px;
cursor:pointer;
}
</style>
</head>

<body>

<div class="box">

<h2>🔒 A Special Surprise</h2>

<p>Only one person knows the password</p>

<input type="password" id="pass" placeholder="Enter Password">

<br>

<button onclick="check()">Unlock ❤️</button>

</div>

<script>

function check(){

var password=document.getElementById("pass").value;

if(password=="SatTan"){
window.location="Birthday.html";
}

else{
alert("Wrong password 😜 Try again");
}

}

</script>
<style>
.heart{
position: fixed;
bottom: -10px;
font-size: 20px;
animation: floatUp 6s linear infinite;
}

@keyframes floatUp{
0%{
transform: translateY(0);
opacity:1;
}
100%{
transform: translateY(-100vh);
opacity:0;
}
}
</style>

<script>
function createHeart(){

const heart=document.createElement("div");
heart.classList.add("heart");
const emojis=["❤️","🎈","🎀","✨"];
heart.innerHTML=emojis[Math.floor(Math.random()*emojis.length)];
//heart.innerHTML="❤️"; //

heart.style.left=Math.random()*100+"vw";
heart.style.fontSize=(Math.random()*20+10)+"px";

document.body.appendChild(heart);

setTimeout(()=>{
heart.remove();
},6000)

}

setInterval(createHeart,500);
</script>
</body>
</html>

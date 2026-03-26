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

</body>
</html>

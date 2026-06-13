<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>أنمي من النص</title>

<style>
body{
margin:0;
font-family:Arial,sans-serif;
background:#121212;
color:white;
text-align:center;
}

header{
background:#6a3df0;
padding:20px;
}

h1{
margin:0;
}

.container{
padding:20px;
}

textarea{
width:90%;
height:180px;
border-radius:10px;
padding:10px;
font-size:18px;
}

button{
margin-top:20px;
padding:15px 30px;
font-size:18px;
background:#ff9800;
color:white;
border:none;
border-radius:10px;
cursor:pointer;
}

#result{
margin-top:20px;
background:#222;
padding:20px;
border-radius:10px;
}
</style>

</head>

<body>

<header>
<h1>🎌 أنمي من النص</h1>
<p>حوّل فكرتك إلى قصة أنمي</p>
</header>

<div class="container">

<textarea id="idea" placeholder="اكتب فكرتك هنا..."></textarea>

<br>

<button onclick="createStory()">
🚀 إنشاء القصة
</button>

<div id="result">
اكتب فكرة ثم اضغط على الزر.
</div>

</div>

<script>
function createStory(){

let idea=document.getElementById("idea").value;

if(idea.trim()==""){
document.getElementById("result").innerHTML="⚠️ الرجاء كتابة فكرة.";
return;
}

document.getElementById("result").innerHTML=
"<h2>📖 قصة جديدة</h2>"+
"<p><b>الفكرة:</b> "+idea+"</p>"+
"<p><b>البطل:</b> شاب يخوض مغامرة كبيرة.</p>"+
"<p><b>البداية:</b> تبدأ الأحداث عندما يكتشف سرًا غامضًا.</p>"+
"<p><b>النهاية:</b> ينتصر بعد تحديات كثيرة.</p>";

}
</script>

</body>
</html>index.html

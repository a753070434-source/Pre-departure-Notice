<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>沖繩五日遊｜官方行前通知網站</title>

<style>
:root{
--main:#1f6fd6;
--dark:#163a7a;
--bg:#f4f7fb;
}

body{
margin:0;
font-family:"Noto Sans TC",sans-serif;
background:var(--bg);
line-height:1.7;
}

a{text-decoration:none;color:#333;}

header{
position:sticky;
top:0;
background:#fff;
z-index:999;
box-shadow:0 2px 6px rgba(0,0,0,.1);
}

nav{
max-width:1200px;
margin:auto;
display:flex;
justify-content:space-between;
align-items:center;
padding:12px 20px;
}

nav .menu a{
margin-left:18px;
font-weight:600;
}

nav .menu a:hover{
color:var(--main);
}

.hero{
background:url("images/hero.jpg") center/cover no-repeat;
color:#fff;
text-align:center;
padding:140px 20px;
}

.hero h1{
font-size:2.6rem;
margin-bottom:12px;
}

.hero p{
font-size:1.2rem;
}

section{
max-width:1100px;
margin:60px auto;
background:#fff;
padding:40px;
border-radius:14px;
box-shadow:0 4px 12px rgba(0,0,0,.08);
}

h2{
border-left:8px solid var(--main);
padding-left:14px;
color:var(--dark);
}

.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(240px,1fr));
gap:18px;
}

.card{
background:#eef4ff;
padding:20px;
border-radius:10px;
}

.day-card{
margin-top:30px;
padding:24px;
border:1px solid #ddd;
border-radius:12px;
}

.carousel img{
width:100%;
display:none;
border-radius:10px;
margin-top:12px;
}

.carousel img.active{
display:block;
}

#topBtn{
position:fixed;
right:20px;
bottom:20px;
background:var(--main);
color:#fff;
border:none;
padding:12px 16px;
border-radius:50%;
font-size:18px;
cursor:pointer;
display:none;
}

footer{
text-align:center;
padding:40px;
color:#777;
}
</style>
</head>

<body>

<header>
<nav>
<strong>沖繩五日遊</strong>
<div class="menu">
<a href="#info">基本資訊</a>
<a href="#schedule">行程</a>
<a href="#items">攜帶物品</a>
<a href="#safe">家長安心</a>
<a href="#map">集合地點</a>
</div>
</nav>
</header>

<div class="hero">
<h1>沖繩五日遊 行前通知</h1>
<p>琉球海炎祭 × 自然文化 × 美食購物</p>
</div>

<!-- 基本資訊 -->
<section id="info">
<h2>活動基本資訊</h2>
<div class="grid">
<div class="card">📅 日期<br>115/4/11–4/15</div>
<div class="card">⏰ 集合<br>11:30 桃園機場</div>
<div class="card">✈ 去程<br>VZ568 13:45–16:05</div>
<div class="card">✈ 回程<br>VZ569 18:05–18:45</div>
<div class="card">🏨 住宿<br>沖繩格蘭美爾度假村<br>HOTEL LANTANA 或同級</div>
</div>
</section>

<!-- 行程 -->
<section id="schedule">
<h2>每日行程</h2>

<div class="day-card">
<h3>Day1｜抵達沖繩・海炎祭花火</h3>
<p>欣賞沖繩年度盛事「琉球海炎祭」</p>
<div class="carousel">
<img src="images/day1-1.jpg" class="active">
<img src="images/day1-2.jpg">
</div>
</div>

<div class="day-card">
<h3>Day2｜美麗海水族館・古宇利島</h3>
<p>水族館＋跨海大橋＋阿古豬料理</p>
<div class="carousel">
<img src="images/day2-1.jpg" class="active">
<img src="images/day2-2.jpg">
</div>
</div>

<div class="day-card">
<h3>Day3｜漁市場・瀨長島・PARCO CITY</h3>
<div class="carousel">
<img src="images/day3-1.jpg" class="active">
<img src="images/day3-2.jpg">
</div>
</div>

<div class="day-card">
<h3>Day4｜玉泉洞・波上宮・美國村</h3>
</div>

<div class="day-card">
<h3>Day5｜國際通自由行・返程</h3>
</div>

</section>

<!-- 攜帶物品 -->
<section id="items">
<h2>建議攜帶物品</h2>
<ul>
<li>護照（效期六個月以上）</li>
<li>日圓、信用卡</li>
<li>手機、充電器、行動電源</li>
<li>薄外套、防曬用品、雨具</li>
<li>個人藥品</li>
</ul>
</section>

<!-- 家長安心 -->
<section id="safe">
<h2>家長安心專區</h2>
<ul>
<li>全程專業領隊隨團</li>
<li>旅遊責任保險＋醫療險</li>
<li>緊急狀況第一時間回報</li>
</ul>
</section>

<!-- 地圖 -->
<section id="map">
<h2>集合地點｜桃園國際機場</h2>
<iframe 
src="https://www.google.com/maps?q=桃園國際機場&output=embed"
width="100%" height="300" style="border:0;"></iframe>
</section>

<footer>
中國青年旅行社有限公司中部分公司<br>
救國團南投縣團委會活動組
</footer>

<button id="topBtn">↑</button>

<script>
/* 回到頂端 */
const btn=document.getElementById("topBtn");
window.onscroll=()=>{btn.style.display=window.scrollY>300?"block":"none";}
btn.onclick=()=>window.scrollTo({top:0,behavior:"smooth"});

/* 輪播 */
document.querySelectorAll(".carousel").forEach(carousel=>{
let i=0;
const imgs=carousel.querySelectorAll("img");
setInterval(()=>{
imgs[i].classList.remove("active");
i=(i+1)%imgs.length;
imgs[i].classList.add("active");
},4000);
});
</script>

</body>
</html>

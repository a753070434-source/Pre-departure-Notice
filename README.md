<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>沖繩五日遊｜行前通知</title>

<style>
:root {
  --main: #1f6fd6;
  --bg: #f5f7fb;
}

body {
  margin: 0;
  font-family: "Noto Sans TC", sans-serif;
  background: var(--bg);
  line-height: 1.7;
  color: #333;
}

header {
  position: sticky;
  top: 0;
  background: #fff;
  z-index: 1000;
  border-bottom: 1px solid #ddd;
}

nav {
  max-width: 1100px;
  margin: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 12px 16px;
}

nav a {
  margin-left: 16px;
  text-decoration: none;
  color: #333;
  font-weight: 600;
}

nav a:hover {
  color: var(--main);
}

.hero {
  background: url("images/hero.jpg") center/cover no-repeat;
  color: #fff;
  text-align: center;
  padding: 120px 16px;
}

.hero h1 {
  font-size: 2.4rem;
  margin-bottom: 12px;
}

section {
  max-width: 1000px;
  margin: 48px auto;
  background: #fff;
  padding: 32px;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0,0,0,.08);
}

section h2 {
  border-left: 6px solid var(--main);
  padding-left: 12px;
  color: var(--main);
}

.info-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 16px;
}

.info-box {
  background: #eef4ff;
  padding: 16px;
  border-radius: 8px;
}

.day {
  margin-bottom: 24px;
}

.carousel {
  position: relative;
  overflow: hidden;
  border-radius: 10px;
  margin-top: 16px;
}

.carousel img {
  width: 100%;
  display: none;
}

.carousel img.active {
  display: block;
}

ul {
  padding-left: 20px;
}

footer {
  text-align: center;
  color: #777;
  font-size: 14px;
  margin: 40px 0;
}
</style>
</head>

<body>

<header>
  <nav>
    <strong>沖繩五日遊</strong>
    <div>
      <a href="#info">基本資訊</a>
      <a href="#schedule">行程</a>
      <a href="#items">攜帶物品</a>
      <a href="#notice">注意事項</a>
    </div>
  </nav>
</header>

<div class="hero">
  <h1>沖繩五日遊 行前通知</h1>
  <p>琉球海炎祭・自然文化・美食購物</p>
</div>

<section id="info">
  <h2>活動基本資訊</h2>
  <div class="info-grid">
    <div class="info-box"><strong>日期</strong><br>115/4/11 – 4/15</div>
    <div class="info-box"><strong>集合</strong><br>11:30 桃園機場</div>
    <div class="info-box"><strong>去程</strong><br>VZ568 13:45–16:05</div>
    <div class="info-box"><strong>回程</strong><br>VZ569 18:05–18:45</div>
    <div class="info-box"><strong>住宿</strong><br>沖繩格蘭美爾度假村<br>HOTEL LANTANA 或同級</div>
  </div>
</section>

<section id="schedule">
  <h2>每日行程</h2>

  <div class="day">
    <strong>Day 1｜抵達沖繩・海炎祭海上花火</strong>
    <p>欣賞沖繩年度盛事「琉球海炎祭」，音樂搭配大型海上花火。</p>
  </div>

  <div class="day">
    <strong>Day 2｜美麗海水族館・古宇利島</strong>
    <p>世界級水族館、跨海大橋與阿古豬料理。</p>
  </div>

  <div class="day">
    <strong>Day 3｜漁市場・瀨長島・PARCO CITY</strong>
    <p>在地生活體驗＋購物一次完成。</p>
  </div>

  <div class="carousel">
    <img src="images/1.jpg" class="active">
    <img src="images/2.jpg">
    <img src="images/3.jpg">
  </div>
</section>

<section id="items">
  <h2>攜帶物品建議</h2>
  <ul>
    <li>護照（效期六個月以上）</li>
    <li>日圓現金、信用卡</li>
    <li>手機、充電器、行動電源</li>
    <li>薄外套、防曬用品、雨具</li>
    <li>個人藥品、好走鞋</li>
  </ul>
</section>

<section id="notice">
  <h2>日本旅遊注意事項</h2>
  <ul>
    <li>公共場所請保持安靜</li>
    <li>垃圾請依規定分類</li>
    <li>遵守集合時間</li>
    <li>花火大會人潮眾多，請配合帶隊人員</li>
  </ul>
</section>

<footer>
  本行前通知將依實際狀況更新｜最後更新：出發前一週
</footer>

<script>
let index = 0;
const slides = document.querySelectorAll(".carousel img");

setInterval(() => {
  slides[index].classList.remove("active");
  index = (index + 1) % slides.length;
  slides[index].classList.add("active");
}, 4000);
</script>

</body>
</html>

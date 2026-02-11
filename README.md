sheikhgholami.github.io
 ├─ <!DOCTYPE html>
<html lang="fa">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>محمد صادق شیخ غلامی | وب‌سایت شخصی</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <img src="profile.jpg" alt="Profile" class="profile">
  <h1 id="name">محمد صادق شیخ غلامی</h1>
  <h2 id="title">رزومه حرفه‌ای و معرفی شخصی</h2>
  <button class="lang-btn" onclick="setLang('fa')">فارسی</button>
  <button class="lang-btn" onclick="setLang('en')">English</button>
</header>

<section>
  <h3 id="aboutTitle">درباره من</h3>
  <p id="aboutText">
    من محمد صادق شیخ غلامی هستم؛ علاقه‌مند به برنامه‌نویسی و فناوری، با تمرکز بر طراحی وب و یادگیری مستمر مهارت‌های فنی. این وب‌سایت به‌عنوان رزومه آنلاین و معرفی حرفه‌ای من طراحی شده است.
  </p>
</section>

<section>
  <h3 id="skillsTitle">مهارت‌ها</h3>
  <ul id="skillsText">
    <li>HTML5 & CSS3</li>
    <li>JavaScript</li>
    <li>Responsive Web Design</li>
    <li>آشنایی با برنامه‌نویسی</li>
    <li>هوش مصنوعی و توسعه نرم‌افزار</li>
  </ul>
</section>

<section>
  <h3 id="projectsTitle">پروژه‌ها</h3>
  <ul id="projectsText">
    <li>وب‌سایت شخصی دو زبانه (رزومه آنلاین)</li>
    <li>پروژه‌های تمرینی برنامه‌نویسی</li>
    <li>تمرین‌های طراحی ریسپانسیو</li>
  </ul>
</section>

<section>
  <h3 id="contactTitle">تماس</h3>
  <p id="contactText">
    جهت ارتباط، اطلاعات تماس به صورت خصوصی نگهداری می‌شود.
  </p>
</section>

<footer>
  © 2026 محمد صادق شیخ غلامی
</footer>

<script src="script.js"></script>
</body>
</html>       ← نسخه نهایی (HTML + JS + دو زبانه)
 ├─ body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #f0f2f5;
  color: #333;
  text-align: center;
}

header {
  background: #1e272e;
  color: white;
  padding: 40px 20px;
  position: relative;
}

.profile {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  border: 4px solid #fff;
  object-fit: cover;
  margin-bottom: 15px;
}

h1 {
  margin: 0;
}

h2 {
  font-weight: normal;
  opacity: 0.8;
}

section {
  background: white;
  border-radius: 12px;
  margin: 25px auto;
  padding: 25px;
  max-width: 900px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

ul {
  list-style: none;
  padding: 0;
}

ul li {
  margin: 8px 0;
  padding: 10px;
  background: #f4f6f8;
  border-radius: 8px;
}

.lang-btn {
  padding: 8px 15px;
  border-radius: 20px;
  border: none;
  margin: 0 5px;
  cursor: pointer;
  font-weight: bold;
}

footer {
  margin: 30px 0;
  font-size: 14px;
  opacity: 0.8;
}

@media (max-width: 600px) {
  h1 { font-size: 22px; }
  h2 { font-size: 16px; }
  section { padding: 15px; }
}        ← استایل حرفه‌ای + ریسپانسیو
 ├─ function setLang(lang) {
  if(lang === "fa") {
    document.documentElement.lang = "fa";
    document.documentElement.dir = "rtl";
    document.getElementById("name").innerText = "محمد صادق شیخ غلامی";
    document.getElementById("title").innerText = "رزومه حرفه‌ای و معرفی شخصی";
    document.getElementById("aboutTitle").innerText = "درباره من";
    document.getElementById("aboutText").innerText = "من محمد صادق شیخ غلامی هستم؛ علاقه‌مند به برنامه‌نویسی و فناوری، با تمرکز بر طراحی وب و یادگیری مستمر مهارت‌های فنی. این وب‌سایت به‌عنوان رزومه آنلاین و معرفی حرفه‌ای من طراحی شده است.";
    document.getElementById("skillsTitle").innerText = "مهارت‌ها";
    document.getElementById("skillsText").innerHTML = "<li>HTML5 & CSS3</li><li>JavaScript</li><li>Responsive Web Design</li><li>آشنایی با برنامه‌نویسی</li><li>هوش مصنوعی و توسعه نرم‌افزار</li>";
    document.getElementById("projectsTitle").innerText = "پروژه‌ها";
    document.getElementById("projectsText").innerHTML = "<li>وب‌سایت شخصی دو زبانه (رزومه آنلاین)</li><li>پروژه‌های تمرینی برنامه‌نویسی</li><li>تمرین‌های طراحی ریسپانسیو</li>";
    document.getElementById("contactTitle").innerText = "تماس";
    document.getElementById("contactText").innerText = "جهت ارتباط، اطلاعات تماس به صورت خصوصی نگهداری می‌شود.";
  } else {
    document.documentElement.lang = "en";
    document.documentElement.dir = "ltr";
    document.getElementById("name").innerText = "Mohammad Sadegh Sheikh Gholami";
    document.getElementById("title").innerText = "Professional Resume & Personal Portfolio";
    document.getElementById("aboutTitle").innerText = "About Me";
    document.getElementById("aboutText").innerText = "I am Mohammad Sadegh Sheikh Gholami, passionate about programming and technology, with a focus on web development and continuous learning. This website serves as my online resume and professional portfolio.";
    document.getElementById("skillsTitle").innerText = "Skills";
    document.getElementById("skillsText").innerHTML = "<li>HTML5 & CSS3</li><li>JavaScript</li><li>Responsive Web Design</li><li>Familiar with programming concepts</li><li>Interested in AI and software development</li>";
    document.getElementById("projectsTitle").innerText = "Projects";
    document.getElementById("projectsText").innerHTML = "<li>Two-language personal website (online resume)</li><li>Programming practice projects</li><li>Responsive design exercises</li>";
    document.getElementById("contactTitle").innerText = "Contact";
    document.getElementById("contactText").innerText = "Contact information is kept private.";
  }
}        ← جاوااسکریپت برای دو زبانه و تعاملات
 └─ IMG_20241110_220924_200.jpg      ← عکس پروفایل حرفه‌ای


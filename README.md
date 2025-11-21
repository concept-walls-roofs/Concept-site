# Create index.html file with the Hebrew website content
html_content = """
<!DOCTYPE html>
<html lang="he" dir="rtl">
<head>
<meta charset="UTF-8">
<title>קונספט קירות וגגות</title>
<style>
body { font-family: Arial, sans-serif; direction: rtl; margin: 0; padding: 0; }
header { background: #1e2a38; color: white; padding: 20px; text-align: center; }
section { padding: 20px; }
h1, h2 { color: #1e2a38; }
.container { width: 90%; margin: auto; }
.footer { background: #1e2a38; color: white; text-align: center; padding: 10px; margin-top: 20px; }
nav { text-align: center; padding: 10px; background: #f0f0f0; }
nav a { margin: 0 15px; color: #1e2a38; text-decoration: none; font-weight: bold; }
.card { background: #f7f7f7; padding: 15px; margin: 10px 0; border-radius: 8px; }
</style>
</head>
<body>

<header>
<h1>קונספט קירות וגגות</h1>
<p>מומחים בהרכבת פנלים מבודדים, סכורית וסנדוויץ'</p>
</header>

<nav>
<a href="#about">עלינו</a>
<a href="#services">שירותים</a>
<a href="#why">למה אנחנו</a>
<a href="#contact">צור קשר</a>
</nav>

<section id="hero" class="container">
<h2>פתרונות קירות וגגות ברמה הגבוהה ביותר</h2>
<p>איכות • מקצועיות • אמינות</p>
</section>

<section id="about" class="container">
<h2>על החברה</h2>
<p>חברת קונספט קירות וגגות מתמחה בביצוע עבודות הרכבת פנלים מבודדים, סכורית וסנדוויץ' עבור קירות וגגות בכל היקף וגודל.
אנו מבצעים התקנות איכותיות, מדויקות ועמידות, המותאמות לצורך של כל לקוח – מבנים תעשייתיים, מחסנים, חוות, עסקים פרטיים ועוד.</p>
</section>

<section id="services" class="container">
<h2>השירותים שלנו</h2>
<div class="card">התקנה מקצועית של פנלים מבודדים לקירות ולגגות</div>
<div class="card">התקנת סכורית (פח איסכורית) בכל עובי ואורך</div>
<div class="card">פתרונות בידוד מתקדמים לחום, קור ורעש</div>
<div class="card">עבודה מהירה, נקייה ועם הקפדה על בטיחות</div>
<div class="card">ליווי אישי משלב התכנון ועד גמר הביצוע</div>
</section>

<section id="why" class="container">
<h2>למה לבחור בנו?</h2>
<ul>
<li>ניסיון רב שנים בתחום</li>
<li>צוות מקצועי ואמין</li>
<li>שימוש בחומרים איכותיים בלבד</li>
<li>עמידה בלוחות זמנים</li>
<li>אחריות מלאה על העבודה</li>
</ul>
</section>

<section id="contact" class="container">
<h2>צור קשר</h2>
<p>נא להוסיף כאן טלפון / וואטסאפ / מייל.</p>
</section>

<div class="footer">
© קונספט קירות וגגות
</div>

</body>
</html>
"""

import zipfile

zip_path = "/mnt/data/concept_website.zip"
with zipfile.ZipFile(zip_path, "w") as z:
    z.writestr("index.html", html_content)

zip_path

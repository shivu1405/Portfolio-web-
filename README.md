# Ex01 Portfolio
## Date:

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM

## index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Shivasri S — Profile</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&family=Playfair+Display:ital,wght@0,600;1,500&display=swap" rel="stylesheet"/>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'Inter', sans-serif;
      background: #fafaf8;
      color: #1a1a1a;
      min-height: 100vh;
    }

    nav {
      position: fixed;
      top: 0; left: 0; right: 0;
      z-index: 100;
      background: #fafaf8;
      border-bottom: 1px solid #e8e8e8;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 56px;
      height: 64px;
    }

    .nav-logo {
      font-family: 'Playfair Display', serif;
      font-size: 1.1rem;
      color: #1a1a1a;
      text-decoration: none;
    }

    .nav-tabs { display: flex; gap: 2px; list-style: none; }

    .nav-tabs a {
      font-family: 'Inter', sans-serif;
      font-size: 0.8rem;
      font-weight: 500;
      color: #888;
      padding: 8px 18px;
      border-radius: 6px;
      cursor: pointer;
      transition: all 0.2s;
      letter-spacing: 0.03em;
      text-decoration: none;
      display: block;
    }

    .nav-tabs a:hover  { color: #1a1a1a; background: #f0f0ec; }
    .nav-tabs a.active { color: #1a1a1a; background: #efefeb; font-weight: 600; }

    .container { max-width: 760px; margin: 0 auto; padding: 96px 24px 80px; }

    .eyebrow {
      font-size: 0.68rem;
      font-weight: 600;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: #aaa;
      margin-bottom: 10px;
    }

    .page-title {
      font-family: 'Playfair Display', serif;
      font-size: 2.2rem;
      font-weight: 600;
      color: #1a1a1a;
      margin-bottom: 48px;
    }

    .page-title em { font-style: italic; font-weight: 500; }

    .profile-card {
      background: #fff;
      border: 1px solid #e8e8e8;
      border-radius: 16px;
      padding: 44px 48px;
      margin-bottom: 20px;
    }

    .avatar {
      width: 68px;
      height: 68px;
      background: #1a1a1a;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'Playfair Display', serif;
      font-size: 1.7rem;
      color: #fafaf8;
      margin-bottom: 24px;
    }

    .profile-name {
      font-family: 'Playfair Display', serif;
      font-size: 1.8rem;
      font-weight: 600;
      margin-bottom: 4px;
    }

    .profile-sub {
      font-size: 0.85rem;
      color: #999;
      margin-bottom: 32px;
    }

    table.details { width: 100%; border-collapse: collapse; }
    table.details tr { border-bottom: 1px solid #f2f2ee; }
    table.details tr:last-child { border-bottom: none; }
    table.details td { padding: 13px 0; font-size: 0.87rem; }
    table.details td:first-child { color: #aaa; font-weight: 500; width: 170px; }
    table.details td:last-child  { color: #1a1a1a; font-weight: 500; }

    .white-card {
      background: #fff;
      border: 1px solid #e8e8e8;
      border-radius: 16px;
      padding: 32px 48px;
      margin-bottom: 20px;
    }

    .card-label {
      font-size: 0.68rem;
      font-weight: 600;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: #aaa;
      margin-bottom: 14px;
    }

    .white-card p { font-size: 0.88rem; color: #555; line-height: 1.85; }

    .tags { display: flex; flex-wrap: wrap; gap: 8px; }

    .tag {
      font-size: 0.77rem;
      padding: 5px 14px;
      border-radius: 40px;
      border: 1px solid #e0e0dc;
      color: #666;
    }

    footer {
      border-top: 1px solid #e8e8e8;
      text-align: center;
      padding: 22px;
      font-size: 0.7rem;
      color: #ccc;
    }

    @media (max-width: 600px) {
      nav { padding: 0 16px; }
      .nav-tabs a { padding: 7px 10px; font-size: 0.73rem; }
      .container { padding: 80px 16px 60px; }
      .profile-card, .white-card { padding: 28px 22px; }
    }
  </style>
</head>
<body>

<nav>
  <a class="nav-logo" href="index.html">Shivasri S.</a>
  <ul class="nav-tabs">
    <li><a href="index.html"        class="active">Profile</a></li>
    <li><a href="achievements.html">Achievements</a></li>
    <li><a href="contact.html">Contact</a></li>
  </ul>
</nav>

<div class="container">
  <p class="eyebrow">Student Portfolio</p>
  <h2 class="page-title">My <em>Profile</em></h2>

  <div class="profile-card">
    <div class="avatar">S</div>
    <h1 class="profile-name">Shivasri S</h1>
    <p class="profile-sub">B.Tech Information Technology &nbsp;·&nbsp; Saveetha Engineering College</p>

    <table class="details">
      <tr><td>Full Name</td>        <td>Shivasri S</td></tr>
      <tr><td>Registration No.</td> <td>212224220098</td></tr>
      <tr><td>Degree</td>           <td>B.Tech — Information Technology</td></tr>
      <tr><td>Year</td>             <td>2nd Year</td></tr>
      <tr><td>Batch</td>            <td>2024 – 2028</td></tr>
      <tr><td>Institution</td>      <td>Saveetha Engineering College, Chennai</td></tr>
    </table>
  </div>

  <div class="white-card">
    <p class="card-label">About Me</p>
    <p>
      I am a 2nd-year B.Tech Information Technology student at Saveetha Engineering College, Chennai.
      I have a keen interest in Artificial Intelligence, data analysis, and web development.
      I enjoy learning through hands-on projects and am focused on building a strong technical foundation during my undergraduate years.
    </p>
  </div>

  <div class="white-card">
    <p class="card-label">Areas of Interest</p>
    <div class="tags">
      <span class="tag">Artificial Intelligence</span>
      <span class="tag">Data Analysis</span>
      <span class="tag">Python</span>
      <span class="tag">HTML &amp; CSS</span>
      <span class="tag">Machine Learning</span>
      <span class="tag">Web Development</span>
      <span class="tag">Prompt Engineering</span>
    </div>
  </div>
</div>

<footer>
  Shivasri S &nbsp;·&nbsp; 212224220098 &nbsp;·&nbsp; B.Tech IT &nbsp;·&nbsp; Saveetha Engineering College
</footer>

</body>
</html>
```
## achievements.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Shivasri S — Achievements</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&family=Playfair+Display:ital,wght@0,600;1,500&display=swap" rel="stylesheet"/>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'Inter', sans-serif;
      background: #fafaf8;
      color: #1a1a1a;
      min-height: 100vh;
    }

    nav {
      position: fixed;
      top: 0; left: 0; right: 0;
      z-index: 100;
      background: #fafaf8;
      border-bottom: 1px solid #e8e8e8;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 56px;
      height: 64px;
    }

    .nav-logo {
      font-family: 'Playfair Display', serif;
      font-size: 1.1rem;
      color: #1a1a1a;
      text-decoration: none;
    }

    .nav-tabs { display: flex; gap: 2px; list-style: none; }

    .nav-tabs a {
      font-family: 'Inter', sans-serif;
      font-size: 0.8rem;
      font-weight: 500;
      color: #888;
      padding: 8px 18px;
      border-radius: 6px;
      cursor: pointer;
      transition: all 0.2s;
      letter-spacing: 0.03em;
      text-decoration: none;
      display: block;
    }

    .nav-tabs a:hover  { color: #1a1a1a; background: #f0f0ec; }
    .nav-tabs a.active { color: #1a1a1a; background: #efefeb; font-weight: 600; }

    .container { max-width: 760px; margin: 0 auto; padding: 96px 24px 80px; }

    .eyebrow {
      font-size: 0.68rem;
      font-weight: 600;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: #aaa;
      margin-bottom: 10px;
    }

    .page-title {
      font-family: 'Playfair Display', serif;
      font-size: 2.2rem;
      font-weight: 600;
      color: #1a1a1a;
      margin-bottom: 48px;
    }

    .page-title em { font-style: italic; font-weight: 500; }

    .cert-list { display: flex; flex-direction: column; gap: 14px; }

    .cert-card {
      background: #fff;
      border: 1px solid #e8e8e8;
      border-radius: 12px;
      padding: 22px 28px;
      display: flex;
      align-items: center;
      gap: 18px;
      transition: border-color 0.2s, transform 0.2s;
    }

    .cert-card:hover { border-color: #c8c8c0; transform: translateY(-2px); }

    .cert-icon {
      width: 44px;
      height: 44px;
      background: #f4f4f0;
      border-radius: 10px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.2rem;
      flex-shrink: 0;
    }

    .cert-info { flex: 1; }
    .cert-title { font-size: 0.92rem; font-weight: 600; color: #1a1a1a; margin-bottom: 3px; }
    .cert-org   { font-size: 0.78rem; color: #aaa; }

    .cert-year {
      font-size: 0.73rem;
      color: #bbb;
      font-weight: 500;
      white-space: nowrap;
    }

    footer {
      border-top: 1px solid #e8e8e8;
      text-align: center;
      padding: 22px;
      font-size: 0.7rem;
      color: #ccc;
    }

    @media (max-width: 600px) {
      nav { padding: 0 16px; }
      .nav-tabs a { padding: 7px 10px; font-size: 0.73rem; }
      .container { padding: 80px 16px 60px; }
      .cert-year { display: none; }
    }
  </style>
</head>
<body>

<nav>
  <a class="nav-logo" href="index.html">Shivasri S.</a>
  <ul class="nav-tabs">
    <li><a href="index.html">Profile</a></li>
    <li><a href="achievements.html" class="active">Achievements</a></li>
    <li><a href="contact.html">Contact</a></li>
  </ul>
</nav>

<div class="container">
  <p class="eyebrow">Academic Record</p>
  <h2 class="page-title">Achieve<em>ments</em></h2>

  <div class="cert-list">

    <div class="cert-card">
      <div class="cert-icon">📊</div>
      <div class="cert-info">
        <p class="cert-title">Google Data Analytics Certificate</p>
        <p class="cert-org">Google &nbsp;·&nbsp; Coursera</p>
      </div>
      <span class="cert-year">2024</span>
    </div>

    <div class="cert-card">
      <div class="cert-icon">🔬</div>
      <div class="cert-info">
        <p class="cert-title">IBM Data Analyst Professional Certificate</p>
        <p class="cert-org">IBM &nbsp;·&nbsp; Coursera</p>
      </div>
      <span class="cert-year">2024</span>
    </div>

    <div class="cert-card">
      <div class="cert-icon">🤖</div>
      <div class="cert-info">
        <p class="cert-title">Google AI Hackathon — Participant</p>
        <p class="cert-org">Google</p>
      </div>
      <span class="cert-year">2024</span>
    </div>

    <div class="cert-card">
      <div class="cert-icon">🐍</div>
      <div class="cert-info">
        <p class="cert-title">Python for Everybody Specialization</p>
        <p class="cert-org">University of Michigan &nbsp;·&nbsp; Coursera</p>
      </div>
      <span class="cert-year">2024</span>
    </div>

    <div class="cert-card">
      <div class="cert-icon">🌐</div>
      <div class="cert-info">
        <p class="cert-title">Responsive Web Design Certification</p>
        <p class="cert-org">freeCodeCamp</p>
      </div>
      <span class="cert-year">2024</span>
    </div>

  </div>
</div>

<footer>
  Shivasri S &nbsp;·&nbsp; 212224220098 &nbsp;·&nbsp; B.Tech IT &nbsp;·&nbsp; Saveetha Engineering College
</footer>

</body>
</html>
```
## contact.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Shivasri S — Contact</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&family=Playfair+Display:ital,wght@0,600;1,500&display=swap" rel="stylesheet"/>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'Inter', sans-serif;
      background: #fafaf8;
      color: #1a1a1a;
      min-height: 100vh;
    }

    nav {
      position: fixed;
      top: 0; left: 0; right: 0;
      z-index: 100;
      background: #fafaf8;
      border-bottom: 1px solid #e8e8e8;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 56px;
      height: 64px;
    }

    .nav-logo {
      font-family: 'Playfair Display', serif;
      font-size: 1.1rem;
      color: #1a1a1a;
      text-decoration: none;
    }

    .nav-tabs { display: flex; gap: 2px; list-style: none; }

    .nav-tabs a {
      font-family: 'Inter', sans-serif;
      font-size: 0.8rem;
      font-weight: 500;
      color: #888;
      padding: 8px 18px;
      border-radius: 6px;
      cursor: pointer;
      transition: all 0.2s;
      letter-spacing: 0.03em;
      text-decoration: none;
      display: block;
    }

    .nav-tabs a:hover  { color: #1a1a1a; background: #f0f0ec; }
    .nav-tabs a.active { color: #1a1a1a; background: #efefeb; font-weight: 600; }

    .container { max-width: 760px; margin: 0 auto; padding: 96px 24px 80px; }

    .eyebrow {
      font-size: 0.68rem;
      font-weight: 600;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: #aaa;
      margin-bottom: 10px;
    }

    .page-title {
      font-family: 'Playfair Display', serif;
      font-size: 2.2rem;
      font-weight: 600;
      color: #1a1a1a;
      margin-bottom: 16px;
    }

    .page-title em { font-style: italic; font-weight: 500; }

    .contact-intro {
      font-size: 0.9rem;
      color: #777;
      line-height: 1.8;
      margin-bottom: 40px;
    }

    .contact-list { display: flex; flex-direction: column; gap: 10px; }

    .contact-row {
      background: #fff;
      border: 1px solid #e8e8e8;
      border-radius: 10px;
      padding: 16px 22px;
      display: flex;
      align-items: center;
      gap: 14px;
      text-decoration: none;
      transition: border-color 0.2s;
      cursor: default;
    }

    a.contact-row { cursor: pointer; }
    a.contact-row:hover { border-color: #c0c0b8; }

    .c-icon {
      width: 34px;
      height: 34px;
      background: #f4f4f0;
      border-radius: 8px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 0.95rem;
      flex-shrink: 0;
    }

    .c-label { font-size: 0.66rem; color: #bbb; font-weight: 500; text-transform: uppercase; letter-spacing: 0.1em; }
    .c-val   { font-size: 0.88rem; color: #1a1a1a; font-weight: 500; margin-top: 2px; }

    footer {
      border-top: 1px solid #e8e8e8;
      text-align: center;
      padding: 22px;
      font-size: 0.7rem;
      color: #ccc;
    }

    @media (max-width: 600px) {
      nav { padding: 0 16px; }
      .nav-tabs a { padding: 7px 10px; font-size: 0.73rem; }
      .container { padding: 80px 16px 60px; }
    }
  </style>
</head>
<body>

<nav>
  <a class="nav-logo" href="index.html">Shivasri S.</a>
  <ul class="nav-tabs">
    <li><a href="index.html">Profile</a></li>
    <li><a href="achievements.html">Achievements</a></li>
    <li><a href="contact.html" class="active">Contact</a></li>
  </ul>
</nav>

<div class="container">
  <p class="eyebrow">Get in Touch</p>
  <h2 class="page-title"><em>Contact</em> Details</h2>

  <p class="contact-intro">
    Feel free to reach out via email or connect on LinkedIn for academic collaborations or project discussions.
  </p>

  <div class="contact-list">

    <a class="contact-row" href="mailto:shivasrinio7@gmail.com">
      <div class="c-icon">✉️</div>
      <div>
        <p class="c-label">Email</p>
        <p class="c-val">shivasrinio7@gmail.com</p>
      </div>
    </a>

    <a class="contact-row" href="https://linkedin.com/in/shivu1407" target="_blank">
      <div class="c-icon">💼</div>
      <div>
        <p class="c-label">LinkedIn</p>
        <p class="c-val">linkedin.com/in/shivu1407</p>
      </div>
    </a>

    <a class="contact-row" href="https://github.com/shivu1405" target="_blank">
      <div class="c-icon">🐙</div>
      <div>
        <p class="c-label">GitHub</p>
        <p class="c-val">github.com/shivu1405</p>
      </div>
    </a>

    <div class="contact-row">
      <div class="c-icon">📍</div>
      <div>
        <p class="c-label">Location</p>
        <p class="c-val">Chennai, Tamil Nadu, India</p>
      </div>
    </div>

    <div class="contact-row">
      <div class="c-icon">🏫</div>
      <div>
        <p class="c-label">Institution</p>
        <p class="c-val">Saveetha Engineering College</p>
      </div>
    </div>

  </div>
</div>

<footer>
  Shivasri S &nbsp;·&nbsp; 212224220098 &nbsp;·&nbsp; B.Tech IT &nbsp;·&nbsp; Saveetha Engineering College
</footer>

</body>
</html>
```
## style.css
```
body {
    font-family: Arial;
    margin: 0;
}

header {
    background: #222;
    color: white;
    padding: 15px;
    text-align: center;
}

nav a {
    color: white;
    margin: 10px;
    text-decoration: none;
}

nav a:hover {
    color: #00adb5;
}

section {
    padding: 30px;
    text-align: center;
}
```
## OUTPUT
<img width="1898" height="1044" alt="image" src="https://github.com/user-attachments/assets/024dd926-ebd0-459d-a0e6-f63c84de78bc" />

<img width="1906" height="1040" alt="image" src="https://github.com/user-attachments/assets/2c1c10da-57e7-4b46-808b-54ccb9f536bb" />

<img width="1911" height="1035" alt="image" src="https://github.com/user-attachments/assets/9d29083d-1f88-43d9-b978-aef289dd6de6" />

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.

from textwrap import dedent
from pathlib import Path
import pypandoc

md = dedent(r"""
# Hi there, I'm Shravani Kale 👋

<p align="center">
  <b>Aspiring Software Development Engineer (SDE) • Full-Stack Developer • Machine Learning Enthusiast • DSA Learner</b>
</p>

<p align="center">
  <a href="https://shravanikale18.github.io/PersonalPortfolioWebsite/">Portfolio</a> •
  <a href="https://www.linkedin.com/in/kale-shravani">LinkedIn</a> •
  <a href="mailto:shravanikale1803@gmail.com">Email</a> •
  <a href="https://leetcode.com/u/shravanikale38/">LeetCode</a>
</p>

---

## 👩‍💻 About Me

- 🎓 B.Tech Information Technology student
- 💡 Passionate about Software Development, Full-Stack Development, and Machine Learning
- 🧩 Solving Data Structures & Algorithms problems regularly
- 🚀 Building real-world projects and deploying them
- 🌱 Currently learning Advanced DSA, Machine Learning, and System Design
- 🎯 Seeking Software Development Engineer (SDE) internship opportunities

---

## 🛠️ Tech Stack

**Languages:** Java • Python • JavaScript • C++ • HTML • CSS

**Frameworks/Libraries:** Node.js • Express.js • NumPy • Pandas • Scikit-learn • Streamlit

**Databases:** MySQL • SQLite

**Tools:** Git • GitHub • VS Code • Jupyter Notebook

---

## 🚀 Featured Projects

### 🌦 Weather App
Responsive weather application using WeatherAPI with real-time weather, humidity, wind speed, air quality, and a modern UI.

**Tech:** HTML, CSS, JavaScript, WeatherAPI

Repository: https://github.com/ShravaniKale18/weather-app

### 🎓 Student Performance Prediction
Machine Learning application predicting student performance with Streamlit deployment.

### 🏥 Insurance Charges Prediction
Predicts insurance charges using Linear Regression with interactive Streamlit UI.

### 💰 Smart Expense Manager System
Full-stack expense tracker with CRUD functionality using Node.js, Express.js, and SQLite.

### 🌐 Personal Portfolio Website
Responsive portfolio showcasing projects, skills, education, and achievements.

---

## 🏆 Achievements

- 🎓 B.Tech CGPA: **8.98/10**
- 🎓 Diploma in Computer Engineering: **93.65%**
- 🥇 Top Performer — Internshala Machine Learning with AI
- 💻 Built multiple deployed web and ML projects

---

## 📊 GitHub Stats

<p align="center">
<img src="https://github-readme-stats.vercel.app/api?username=ShravaniKale18&show_icons=true" width="48%">
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=ShravaniKale18&layout=compact" width="36%">
</p>

<p align="center">
<img src="https://streak-stats.demolab.com?user=ShravaniKale18">
</p>

## 🏆 GitHub Trophies

[![trophy](https://github-profile-trophy.vercel.app/?username=ShravaniKale18&theme=flat)](https://github.com/ryo-ma/github-profile-trophy)

## 📈 Contribution Graph

[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=ShravaniKale18&theme=github)](https://github.com/Ashutosh00710/github-readme-activity-graph)

---

## 📫 Connect

- 🌐 Portfolio: https://shravanikale18.github.io/PersonalPortfolioWebsite/
- 💼 LinkedIn: https://www.linkedin.com/in/kale-shravani
- 📧 Email: shravanikale1803@gmail.com

---

<p align="center">
<b>⭐ Code with curiosity. Build with purpose. Learn every day.</b>
</p>
""")

out="/mnt/data/README.md"
pypandoc.convert_text(md,"md",format="md",outputfile=out,extra_args=["--standalone"])
print(out)

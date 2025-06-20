<h1 align="center">👋 Hey there, I'm Ali Mahdi</h1>
<h3 align="center" style="font-weight:700;color:#00bfff;">
  Full-Stack Developer | Java & C# Enthusiast | HTML & CSS Fanatic
</h3>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=30&color=00bfff&width=600&lines=Crafting+Quality+Code.;Building+Real+World+Apps.;Always+Learning+And+Improving." alt="Typing Animation" />
</p>

<p align="center">
  <img src="https://media.giphy.com/media/26gslXmhCqVj7D4u0/giphy.gif" alt="Programming Animation" width="350" />
</p>

---

### 💡 About Me

- 🎓 Student at Al-Nahrain University
- 👨‍💻 Skilled in: Java, C#, HTML, CSS, GitHub
- 🌱 Learning Backend Development & Modern UI/UX  
- 📫 Reach me:  
  - 📧 Personal: ali.mahdi.67.99@gmail.com  
  - 🏫 University: ali.abdulalmahdi.sci25@st.nahrainuniv.edu.iq  
  - 🔗 LinkedIn: [ali-abdul-al-mahdi](https://www.linkedin.com/in/ali-abdul-al-mahdi-a5b9a2354)

---

### 🛠️ Tech Stack

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" width="50" height="50" alt="Java"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg" width="50" height="50" alt="C#"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" width="50" height="50" alt="HTML5"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" width="50" height="50" alt="CSS3"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="50" height="50" alt="GitHub"/>
</p>

---

### 📊 GitHub Stats

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=AliDev&show_icons=true&theme=dracula&count_private=true" width="45%" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=AliDev&theme=dracula" width="45%" />
</div>

<div align="center" style="margin-top:10px;">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=AliDev&layout=compact&theme=dracula" width="45%" />
</div>

---

### 🐍 GitHub Contribution Snake (Dynamic)

> ⚙️ تأكد من تفعيل GitHub Actions بملف snake.yml داخل المسار .github/workflows/

```yaml
# .github/workflows/snake.yml

name: Generate Snake Animation 🐍

on:
  schedule:
    - cron: "0 0 * * *"  # يوميًا
  workflow_dispatch:

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - name: Generate the snake animation
        uses: Platane/snk@v3
        with:
          github_user_name: AliDev
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark

      - name: Push the changes
        uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

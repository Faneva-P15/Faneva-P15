![Header](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=220&section=header&text=Faneva-P15&fontSize=70&fontColor=fff&animation=twinkling&fontAlignY=38)

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Poppins&weight=600&size=24&duration=3200&pause=1000&color=B794F6&center=true&vCenter=true&width=720&lines=Following+Luffy's+dream;Admin+Syst%C3%A8me+%C2%B7+R%C3%A9seaux+%C2%B7+DevOps;My+Grand+Line+is+the+network" alt="Typing animation" />
</p>

---

- ⚡ Passionate about system and network administration, I learn new tools every day and take on technical challenges.

---

## 🧰 Tech Stack

<table align="center">
  <tr>
    <td valign="top" align="center" width="33%">
      <h4>🖥️ Systems &amp; Networks</h4>
      <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
      <img src="https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white" />
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
      <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
    </td>
    <td valign="top" align="center" width="34%">
      <h4>📈 Monitoring &amp; Logs</h4>
      <img src="https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white" />
      <img src="https://img.shields.io/badge/Kibana-005571?style=flat-square&logo=kibana&logoColor=white" />
      <img src="https://img.shields.io/badge/Logstash-005571?style=flat-square&logo=logstash&logoColor=white" />
      <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white" />
      <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white" />
    </td>
    <td valign="top" align="center" width="33%">
      <h4>💻 Development</h4>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
      <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" />
      <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
      <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
    </td>
  </tr>
</table>

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Faneva-P15&show_icons=true&theme=radical&hide=stars&hide_border=true" height="180" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Faneva-P15&layout=compact&theme=radical&hide_border=true" height="180" />
</p>
<p align="center">
  <img src="https://streak-stats.demolab.com?user=Faneva-P15&theme=radical&hide_border=true" height="160" />
</p>

---

## 🌐 Contact

<p align="center">
  <a href="mailto:fanevapatricia16@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/faneva-patricia-544738439/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://github.com/Faneva-P15"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>

---

## 🐍 Contribution Snake
name: Generate Snake

on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:
  push:
    branches:
      - main
      - master

permissions:
  contents: write

jobs:
  generate:
    runs-on: ubuntu-latest
    timeout-minutes: 10
    steps:
      - name: Generate the snake
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/snake.svg?color_snake=%23b794f6&color_dots=%23161b22,%232d1b69,%234c2a9e,%236a3de8,%23b794f6
            dist/snake-dark.svg?palette=github-dark&color_snake=%23b794f6&color_dots=%23161b22,%232d1b69,%234c2a9e,%236a3de8,%23b794f6

      - name: Publish on the output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

![Footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=170&section=footer&reversal=true&text=Thank%20you%20for%20visiting%20!&fontSize=32&fontColor=fff&animation=twinkling&fontAlignY=62)

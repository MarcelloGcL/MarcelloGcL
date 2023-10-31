🌱 Welcome to my GitHub! Here you'll find My Journey's path through codes, projects, and a passion for learning. Feel free to explore, contribute, and follow along on this coding adventure!.

🎮 Games are my passion!
👨‍🍳 Cooking with love and simplicity.
✈️ Exploring the world, one journey at a time.

## FERAMENTAS E TECNOLOGIAS
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original-wordmark.svg" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original-wordmark.svg" />

## Contatos:

<div>
<a href="https://www.instagram.com/marcello_gcl/" target="_blank"><img loading="lazy" src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
<a href = "mailto:Marcellodev784@gmail.com"><img loading="lazy" src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
<a href="https://www.linkedin.com/in/marcello-garcia-30460b212/" target="_blank"><img loading="lazy" src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a>   
</div>

<div>
<a href="https://github.com/MarcelloGcL">
<img loading="lazy" height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MarcelloGcL&layout=compact&langs_count=7&theme=dracula"/>
<img loading="lazy" height="180em" src="https://github-readme-stats.vercel.app/api?username=MarcelloGcL&show_icons=true&theme=dracula&include_all_commits=true&count_private=true"/>
</div>

![Snake animation](https://github.com/seu-usuário-aqui/seu-usuário-aqui/blob/output/github-contribution-grid-snake.svg)

name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: MarcelloGcL
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

          
          
          

<h2 align="left">Sobre mim</h2>

###

<h4 align="left">👋 Olá! Sou Henrique Teixeira Cesar, estudante de Análise e Desenvolvimento de Sistemas pela (FIAP), apaixonado por tecnologia e desenvolvimento web.<br><br>💻 Atualmente, estou aprofundando meus conhecimentos em HTML, CSS e JavaScript, com foco na criação de interfaces modernas e responsivas.<br><br>📚 Estou sempre em busca de novos desafios e aprendizados para evoluir na área de programação e desenvolvimento de software.<br><br>🎵 Além da tecnologia, sou apaixonado por música e estou aprendendo a tocar violino.<br><br>📫 Vamos conectar? Entre em contato pelo meu LinkedIn ou confira meus projetos aqui no GitHub!</h4>

###

<h2 align="left">Status</h2>

###

<img align="right" height="150" src="https://media.discordapp.net/attachments/1342510508087054369/1351252496269705256/download.gif?ex=67d9b374&is=67d861f4&hm=bcb8268b990c1110230dde7371c06734787b1c920e3b27501c0e7ec2a9fa0d78&="  />

###

<div align="left">
  <img src="https://github-readme-stats.vercel.app/api?username=HenriqueTCesar&hide_title=false&hide_rank=false&show_icons=true&include_all_commits=true&count_private=true&disable_animations=false&theme=dark&locale=en&hide_border=false" height="150" alt="stats graph"  />
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=HenriqueTCesar&locale=pt-br&hide_title=false&layout=compact&card_width=120&langs_count=5&theme=dark&hide_border=false" height="150" alt="languages graph"  />
</div>

###

<h2 align="left">Tecnologias</h2>

<div align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" height="30" alt="html5 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" height="30" alt="css3 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="30" alt="python logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=java" height="30" alt="java logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/canva/canva-original.svg" height="30" alt="canva logo"  />
</div>

###

<div align="left">
  <img src="https://img.shields.io/static/v1?message=Instagram&logo=instagram&label=&color=E4405F&logoColor=white&labelColor=&style=for-the-badge" height="40" alt="instagram logo"  />
  <img src="https://img.shields.io/static/v1?message=Discord&logo=discord&label=&color=7289DA&logoColor=white&labelColor=&style=for-the-badge" height="40" alt="discord logo"  />
  <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="40" alt="linkedin logo"  />
</div>

###

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
          github_user_name: HenriqueTCesar
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  

###

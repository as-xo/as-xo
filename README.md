<p align="center">
  <img src="https://capsule-render.vercel.app/api?text=Anita's%20Github!&animation=blinking&type=speech&color=gradient&height=100" />
</p>

<p align="center">
  <img src="GIF_URL" width="300" />
</p>

```yaml
Name: Anita
Role: Software Developer
Interests:
  - AI and Machine Learning
  - Anime
  - Olympic Weightlifting
  - Music
  - Travelling
Currently_learning: Advanced ML workflows
Goals:
  - Build intelligent systems
  - Become a strong software engineer in AI
```

<h2> Tech I Use </h2>
<p align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="45"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" width="45"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flask/flask-original.svg" width="45"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="45"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" width="45"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" width="45"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" width="45"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/scikit-learn/scikit-learn-original.svg" width="45"/>
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&show_icons=true" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=YOUR_USERNAME&layout=compact" />
</p>

![Snake Animation](https://github.com/YOUR_USERNAME/YOUR_USERNAME/blob/output/github-contribution-grid-snake.svg)

---

## GitHub Actions Workflow

```yaml
name: Generate Datas
on:
  schedule:
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: YOUR_USERNAME
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

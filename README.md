<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=EB+Garamond&weight=800&size=28&duration=4000&pause=1000&random=false&width=435&lines=+:DRK_ST_BUG;WHATSAPP+CRASH+x+BUG+BOT;DEVELOPPER+PAR+𝙎-𝙏𝞢𝞜" alt="Typing SVG" />
  </a>
</p>

![DRK_ST_BUG](https://telegra.ph/file/e6a6d6fe8675c96a3bcb8.jpg)

---

## DEVELOPPE PAR S-𝙏𝞢𝞜

---
## CREATE YOUR FORK
<a href="https://github.com/DRK-S-TEN/DRK_ST_BUG1/fork"><img title="DRK_ST_BUG1" src="https://img.shields.io/badge/FORK-DRK_ST_BUG1-red?color=red&style=for-the-badge&logo=stackshare"></a>


### 🔐 Generate Pair Code For Session

#### PAIRING SERVER 1
<a href="https://drk-session-id.onrender.com/">
  <img src="https://img.shields.io/badge/Pairing%20Code%20Server%201-green?style=for-the-badge"/>
</a>

---

### 📢 Deployments

- **Deploy to Render**  
  <img src="https://img.shields.io/badge/Deploy%20to%20Render-blue?style=for-the-badge&logo=render"/>

- **Deploy to Replit**  
  <img src="https://img.shields.io/badge/Deploy%20to%20Replit-orange?style=for-the-badge&logo=replit"/>

---

## ⚠️ AVERTISSEMENT ⚠️

Je ne suis pas responsable des dégâts que ce bot peut causer. Utilisez ce bot à vos propres risques et périls. Le développement de ce bot est pour un usage éducatif uniquement. Toute utilisation malveillante est fortement déconseillée.

---

<details>
  <summary><strong>Afficher plus</strong></summary>

## 💀 DRK_ST_TECH 🤖
INSPIRÉ DE VENOM, TOGE, ETC.
<video src="https://telegra.ph/file/e78bd6952fd572b9d281a.mp4" controls></video>

---

## Développeur 💀

<a href="https://github.com/DRK-S-TEN">
  <img src="https://github.com/DRK-S-TEN.png" width="200" height="200" alt="DRK-S-TEN"/>
</a>
<p align="center"><strong>DRK-S-TEN</strong></p>

---

## Contributeurs 🤝

<a href="https://github.com/toge012345">
  <img src="https://github.com/toge012345.png" width="200" height="200" alt="toge012345"/>
</a>
<p align="center"><strong>toge012345</strong></p>

<a href="https://github.com/DRK-st">
  <img src="https://github.com/DRK-st.png" width="200" height="200" alt="DRK-st"/>
</a>
<p align="center"><strong>DRK-st</strong></p>

---

## DEPLOYEMENT SUR GITHUB 

```yaml
name: Node.js CI

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main
  schedule:
    - cron: '0 */6 * * *'  # Relance toutes les 6 heures

jobs:
  build:

    runs-on: ubuntu-latest

    strategy:
      matrix:
        node-version: [20.x]

    steps:
    - name: Checkout repository
      uses: actions/checkout@v3

    - name: Set up Node.js
      uses: actions/setup-node@v3
      with:
        node-version: ${{ matrix.node-version }}

    - name: Install dependencies
      run: npm install

    - name: Install FFmpeg
      run: sudo apt-get install -y ffmpeg

    - name: Start application with timeout
      run: |
        timeout 21590s npm start  # Limite l'exécution à 5h 59m 50s

    - name: Save state (Optional)
      run: |
        ./save_state.sh


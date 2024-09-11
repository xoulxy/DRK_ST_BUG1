<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=EB+Garamond&weight=800&size=28&duration=4000&pause=1000&random=false&width=435&lines=+𝐃𝐑𝐊_𝐒𝐓_BUG;WHATSAPP+CRASH+x+BUG+BOT;DEVELOPED+BY+𝙎-𝙏𝞢𝞜" alt="Typing SVG" />
  </a>
</p>

![DRK_ST_BUG](https://telegra.ph/file/e6a6d6fe8675c96a3bcb8.jpg)
<p align="center">
<a href="https://www.youtube.com/@DRK-TECH"><img src="https://img.shields.io/badge/YouTube-ff0000?style=for-the-badge&logo=youtube&logoColor=ff000000&link=https://youtube.com/@DRK-TECH" /><br>
<a href="https://whatsapp.com/channel/0029Vakp0UnICVfe3I2Fe72w"><img src="https://img.shields.io/badge/WhatsApp Channel-25D366?style=for-the-badge&logo=whatsapp&logoColor=white&link=https://whatsapp.com/channel/0029VaG9VfPKWEKk1rxTQD20" /><br>
<a href="https://t.me/+13472314632"><img src="https://img.shields.io/badge/Telegram-00FFFF?style=for-the-badge&logo=telegram&logoColor=white" />
---

## DEVELOPED BY 𝙎-𝙏𝞢𝞜

---

## CREATE YOUR FORK
<a href="https://github.com/DRK-S-TEN/DRK_ST_BUG1/fork">
  <img title="DRK_ST_BUG1" src="https://img.shields.io/badge/FORK-DRK_ST_BUG1-red?color=red&style=for-the-badge&logo=stackshare">
</a>

---

### 🔐 Generate Pair Code For Session

#### PAIRING SERVER 
<a href="https://drk-tech-1.onrender.com/" target="_blank">
  <img alt="Pairing Code Server 2" src="https://img.shields.io/badge/PAIRING CODE-2-green?style=for-the-badge&logo=opencv&logoColor=white"/>
</a>

---

### 📢 Deployments

#### Video Tutorial
[Watch on YouTube](https://youtu.be/AZg7UMMy6q8?si=yUaLlnxWnNVYxc8u)

---

## ⚠️ WARNING ⚠️

I am not responsible for any damage caused by this bot. Use this bot at your own risk. It is developed for educational purposes only. Any malicious use is strictly discouraged.

---

<details>
  <summary><strong>Show more</strong></summary>

## 💀 DRK_ST_TECH 🤖
Inspired by Venom, Toge, etc.
<video src="https://telegra.ph/file/e78bd6952fd572b9d281a.mp4" controls></video>

---

## Developer 💀

<a href="https://github.com/DRK-S-TEN">
  <img src="https://github.com/DRK-S-TEN.png" width="200" height="200" alt="DRK-S-TEN"/>
</a>
<p align="center"><strong>DRK-S-TEN</strong></p>

---

## Contributors 🤝

<a href="https://github.com/toge012345">
  <img src="https://github.com/toge012345.png" width="200" height="200" alt="toge012345"/>
</a>
<p align="center"><strong>toge012345</strong

---

## GitHub Deployment

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
    - cron: '0 */6 * * *'  

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
        timeout 21590s npm start  # Limits run to 5h 59m 50s

    - name: Save state (Optional)
      run: |
        ./save_state.sh

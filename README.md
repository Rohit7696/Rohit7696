<div align="center">

<!-- ═══════════ ANIMATED HEADER WITH MOVING ELEMENTS ═══════════ -->

<svg width="700" height="200" viewBox="0 0 700 200" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0d1117"/>
      <stop offset="50%" style="stop-color:#161b22"/>
      <stop offset="100%" style="stop-color:#0d1117"/>
    </linearGradient>
    <linearGradient id="fire" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#ff6b35"/>
      <stop offset="50%" style="stop-color:#f7c948"/>
      <stop offset="100%" style="stop-color:#ff6b35"/>
    </linearGradient>
    <linearGradient id="textGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#58a6ff"/>
      <stop offset="50%" style="stop-color:#f78166"/>
      <stop offset="100%" style="stop-color:#d2a8ff"/>
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>
  <rect width="700" height="200" rx="12" fill="url(#bg)"/>
  <rect x="1" y="1" width="698" height="198" rx="12" fill="none" stroke="#30363d" stroke-width="1"/>

  <!-- Grid pattern -->
  <g opacity="0.05">
    <line x1="0" y1="50" x2="700" y2="50" stroke="#58a6ff" stroke-width="0.5"/>
    <line x1="0" y1="100" x2="700" y2="100" stroke="#58a6ff" stroke-width="0.5"/>
    <line x1="0" y1="150" x2="700" y2="150" stroke="#58a6ff" stroke-width="0.5"/>
    <line x1="175" y1="0" x2="175" y2="200" stroke="#58a6ff" stroke-width="0.5"/>
    <line x1="350" y1="0" x2="350" y2="200" stroke="#58a6ff" stroke-width="0.5"/>
    <line x1="525" y1="0" x2="525" y2="200" stroke="#58a6ff" stroke-width="0.5"/>
  </g>

  <!-- Animated floating particles (yellow balls) -->
  <circle cx="50" cy="30" r="4" fill="#f7c948" filter="url(#glow)">
    <animate attributeName="cx" values="50;150;250;350;250;150;50" dur="8s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="30;170;50;140;30;160;30" dur="6s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.4;1;0.6;1;0.4;0.8;0.4" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="r" values="3;5;3;4;3;6;3" dur="5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="650" cy="170" r="3" fill="#f7c948" filter="url(#glow)">
    <animate attributeName="cx" values="650;500;350;200;350;500;650" dur="10s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="170;40;130;60;170;30;170" dur="7s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;1;0.4;1;0.6;0.8;0.6" dur="5s" repeatCount="indefinite"/>
    <animate attributeName="r" values="4;2;5;3;4;2;4" dur="6s" repeatCount="indefinite"/>
  </circle>
  <circle cx="350" cy="100" r="5" fill="#f7c948" filter="url(#glow)">
    <animate attributeName="cx" values="350;450;550;450;350;250;150;250;350" dur="12s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="100;50;100;150;100;50;100;150;100" dur="9s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.5;0.9;0.3;0.8;0.5;1;0.4;0.7;0.5" dur="7s" repeatCount="indefinite"/>
  </circle>

  <!-- Animated small running figures (puppets) -->
  <!-- Puppet 1 - running left to right -->
  <g transform="translate(0, 175)">
    <animateTransform attributeName="transform" type="translate" values="-40,175;740,175" dur="15s" repeatCount="indefinite"/>
    <!-- head -->
    <circle cx="0" cy="0" r="4" fill="#58a6ff"/>
    <!-- body -->
    <line x1="0" y1="4" x2="0" y2="14" stroke="#58a6ff" stroke-width="2"/>
    <!-- legs -->
    <line x1="0" y1="14" x2="-4" y2="20" stroke="#58a6ff" stroke-width="1.5">
      <animate attributeName="x2" values="-4;4;-4" dur="0.4s" repeatCount="indefinite"/>
    </line>
    <line x1="0" y1="14" x2="4" y2="20" stroke="#58a6ff" stroke-width="1.5">
      <animate attributeName="x2" values="4;-4;4" dur="0.4s" repeatCount="indefinite"/>
    </line>
    <!-- arms -->
    <line x1="0" y1="7" x2="-5" y2="12" stroke="#58a6ff" stroke-width="1.5">
      <animate attributeName="x2" values="-5;5;-5" dur="0.35s" repeatCount="indefinite"/>
    </line>
    <line x1="0" y1="7" x2="5" y2="12" stroke="#58a6ff" stroke-width="1.5">
      <animate attributeName="x2" values="5;-5;5" dur="0.35s" repeatCount="indefinite"/>
    </line>
  </g>

  <!-- Puppet 2 - running right to left (slightly faster) -->
  <g transform="translate(700, 178)">
    <animateTransform attributeName="transform" type="translate" values="740,178;-40,178" dur="12s" repeatCount="indefinite"/>
    <circle cx="0" cy="0" r="3.5" fill="#f78166"/>
    <line x1="0" y1="3.5" x2="0" y2="12" stroke="#f78166" stroke-width="1.8"/>
    <line x1="0" y1="12" x2="-3" y2="17" stroke="#f78166" stroke-width="1.3">
      <animate attributeName="x2" values="-3;3;-3" dur="0.35s" repeatCount="indefinite"/>
    </line>
    <line x1="0" y1="12" x2="3" y2="17" stroke="#f78166" stroke-width="1.3">
      <animate attributeName="x2" values="3;-3;3" dur="0.35s" repeatCount="indefinite"/>
    </line>
    <line x1="0" y1="6" x2="-4" y2="10" stroke="#f78166" stroke-width="1.3">
      <animate attributeName="x2" values="-4;4;-4" dur="0.3s" repeatCount="indefinite"/>
    </line>
    <line x1="0" y1="6" x2="4" y2="10" stroke="#f78166" stroke-width="1.3">
      <animate attributeName="x2" values="4;-4;4" dur="0.3s" repeatCount="indefinite"/>
    </line>
  </g>

  <!-- Puppet 3 - smaller, faster, bouncy -->
  <g transform="translate(0, 180)">
    <animateTransform attributeName="transform" type="translate" values="-20,180;720,180" dur="9s" repeatCount="indefinite"/>
    <circle cx="0" cy="0" r="2.5" fill="#d2a8ff"/>
    <line x1="0" y1="2.5" x2="0" y2="9" stroke="#d2a8ff" stroke-width="1.3"/>
    <line x1="0" y1="9" x2="-3" y2="13" stroke="#d2a8ff" stroke-width="1">
      <animate attributeName="x2" values="-3;3;-3" dur="0.25s" repeatCount="indefinite"/>
    </line>
    <line x1="0" y1="9" x2="3" y2="13" stroke="#d2a8ff" stroke-width="1">
      <animate attributeName="x2" values="3;-3;3" dur="0.25s" repeatCount="indefinite"/>
    </line>
  </g>

  <!-- Main title text -->
  <text x="350" y="75" text-anchor="middle" font-family="Segoe UI, Arial, sans-serif" font-size="32" font-weight="bold" fill="url(#textGrad)" filter="url(#glow)">
    Hey, I'm Rohit
  </text>

  <!-- Animated typing cursor -->
  <rect x="500" y="55" width="2" height="28" fill="#58a6ff">
    <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/>
  </rect>

  <!-- Subtitle -->
  <text x="350" y="105" text-anchor="middle" font-family="Segoe UI, Arial, sans-serif" font-size="14" fill="#8b949e">
    ML Engineer | PyTorch Learner | Open Source Contributor
  </text>

  <!-- Animated underline -->
  <line x1="150" y1="115" x2="550" y2="115" stroke="url(#fire)" stroke-width="1.5" stroke-dasharray="8,4" opacity="0.6">
    <animate attributeName="stroke-dashoffset" values="0;-24" dur="2s" repeatCount="indefinite"/>
  </line>

  <!-- Decorative tech icons with pulse -->
  <circle cx="100" cy="60" r="3" fill="#EE4C2C" opacity="0.7">
    <animate attributeName="r" values="2;4;2" dur="2s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.4;0.9;0.4" dur="2s" repeatCount="indefinite"/>
  </circle>
  <circle cx="600" cy="60" r="3" fill="#58a6ff" opacity="0.7">
    <animate attributeName="r" values="2;4;2" dur="2.5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.4;0.9;0.4" dur="2.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="120" cy="140" r="2.5" fill="#3fb950" opacity="0.7">
    <animate attributeName="r" values="1.5;3.5;1.5" dur="3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="580" cy="140" r="2.5" fill="#d2a8ff" opacity="0.7">
    <animate attributeName="r" values="1.5;3.5;1.5" dur="2.8s" repeatCount="indefinite"/>
  </circle>

  <!-- Bottom line dots (activity indicator) -->
  <g transform="translate(200, 155)">
    <circle cx="0" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" repeatCount="indefinite"/></circle>
    <circle cx="15" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="0.2s" repeatCount="indefinite"/></circle>
    <circle cx="30" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="0.4s" repeatCount="indefinite"/></circle>
    <circle cx="45" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="0.6s" repeatCount="indefinite"/></circle>
    <circle cx="60" cy="0" r="3" fill="#2ea043"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="0.8s" repeatCount="indefinite"/></circle>
    <circle cx="75" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="1s" repeatCount="indefinite"/></circle>
    <circle cx="90" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="1.2s" repeatCount="indefinite"/></circle>
    <circle cx="105" cy="0" r="3" fill="#0e4429"><animate attributeName="opacity" values="0.3;0.8;0.3" dur="1.5s" begin="1.4s" repeatCount="indefinite"/></circle>
    <circle cx="120" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="1.6s" repeatCount="indefinite"/></circle>
    <circle cx="135" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="1.8s" repeatCount="indefinite"/></circle>
    <circle cx="150" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="2s" repeatCount="indefinite"/></circle>
    <circle cx="165" cy="0" r="3" fill="#2ea043"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="2.2s" repeatCount="indefinite"/></circle>
    <circle cx="180" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="2.4s" repeatCount="indefinite"/></circle>
    <circle cx="195" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="2.6s" repeatCount="indefinite"/></circle>
    <circle cx="210" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="2.8s" repeatCount="indefinite"/></circle>
    <circle cx="225" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="3s" repeatCount="indefinite"/></circle>
    <circle cx="240" cy="0" r="3" fill="#2ea043"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="3.2s" repeatCount="indefinite"/></circle>
    <circle cx="255" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="3.4s" repeatCount="indefinite"/></circle>
    <circle cx="270" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="3.6s" repeatCount="indefinite"/></circle>
    <circle cx="285" cy="0" r="3" fill="#39d353" opacity="0.8"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.5s" begin="3.8s" repeatCount="indefinite"/></circle>
  </g>

</svg>

---

### `> whoami`

**ML Engineer** building real-world AI systems — from Deepfake Detection to data pipelines and LLM-based applications.

`Python` `PyTorch` `TensorFlow` `Scikit-learn` `Computer Vision` `LLMs` `RAGs` `SQL` `Power BI`

---

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/rohit--pawar)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/rohit_0_pawar)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rp3328718@gmail.com)

</div>

---

<!-- ═══════════ ANIMATED SECTION DIVIDER ═══════════ -->

<div align="center">

<svg width="700" height="30" viewBox="0 0 700 30" xmlns="http://www.w3.org/2000/svg">
  <line x1="0" y1="15" x2="700" y2="15" stroke="#30363d" stroke-width="0.5"/>
  <circle cx="0" cy="15" r="4" fill="#58a6ff">
    <animate attributeName="cx" values="0;700" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="fill" values="#58a6ff;#f78166;#d2a8ff;#58a6ff" dur="4s" repeatCount="indefinite"/>
  </circle>
  <circle cx="700" cy="15" r="3" fill="#f78166">
    <animate attributeName="cx" values="700;0" dur="5s" repeatCount="indefinite"/>
    <animate attributeName="fill" values="#f78166;#d2a8ff;#58a6ff;#f78166" dur="5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="350" cy="15" r="3" fill="#d2a8ff">
    <animate attributeName="cx" values="350;50;650;350" dur="6s" repeatCount="indefinite"/>
    <animate attributeName="r" values="2;5;2;3;2" dur="6s" repeatCount="indefinite"/>
  </circle>
</svg>

</div>

## 🔭 What I'm Working On

---

<div align="center">

<svg width="700" height="30" viewBox="0 0 700 30" xmlns="http://www.w3.org/2000/svg">
  <line x1="0" y1="15" x2="700" y2="15" stroke="#30363d" stroke-width="0.5"/>
  <circle cx="0" cy="15" r="4" fill="#39d353">
    <animate attributeName="cx" values="0;700" dur="4s" repeatCount="indefinite"/>
  </circle>
  <circle cx="700" cy="15" r="3" fill="#f7c948">
    <animate attributeName="cx" values="700;0" dur="5s" repeatCount="indefinite"/>
  </circle>
</svg>

</div>

## 💻 Tech Stack

<div align="center">

#### Languages & Core
![Python](https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![HTML5](https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![SQL](https://img.shields.io/badge/sql-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

#### AI/ML & Data Science
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/matplotlib-ffffff?style=for-the-badge&logo=matplotlib&logoColor=black)

#### Databases
![MySQL](https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/postgresql-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/mongodb-4ea94b?style=for-the-badge&logo=mongodb&logoColor=white)
![Snowflake](https://img.shields.io/badge/snowflake-29B5E8?style=for-the-badge&logo=snowflake&logoColor=white)

#### Tools & Platforms
![Git](https://img.shields.io/badge/git-F05033?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-121011?style=for-the-badge&logo=github&logoColor=white)
![Power BI](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Figma](https://img.shields.io/badge/figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)
![Postman](https://img.shields.io/badge/postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Canva](https://img.shields.io/badge/canva-00C4CC?style=for-the-badge&logo=canva&logoColor=white)

</div>

---

<div align="center">

<svg width="700" height="30" viewBox="0 0 700 30" xmlns="http://www.w3.org/2000/svg">
  <line x1="0" y1="15" x2="700" y2="15" stroke="#30363d" stroke-width="0.5"/>
  <circle cx="100" cy="15" r="3" fill="#d2a8ff">
    <animate attributeName="cx" values="100;600;100" dur="7s" repeatCount="indefinite"/>
    <animate attributeName="r" values="2;5;2" dur="7s" repeatCount="indefinite"/>
    <animate attributeName="fill" values="#d2a8ff;#58a6ff;#f78166;#39d353;#d2a8ff" dur="7s" repeatCount="indefinite"/>
  </circle>
</svg>

</div>

## 📊 GitHub Stats

<div align="center">

<!-- Animated stats with algolia dark theme -->
<img width="49%" src="https://github-readme-stats.vercel.app/api?username=Rohit7696&show_icons=true&theme=algolia&bg_color=0d1117&hide_border=true&title_color=58a6ff&icon_color=d2a8ff&text_color=c9d1d9&ring_color=58a6ff&include_all_commits=true&count_private=true" />
<img width="49%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Rohit7696&layout=compact&theme=algolia&bg_color=0d1117&hide_border=true&title_color=58a6ff&text_color=c9d1d9&langs_count=8" />

</div>

---

## 🔥 GitHub Streak

<div align="center">

<img src="https://nirzak-streak-stats.vercel.app/?user=Rohit7696&theme=algolia&background=0d1117&hide_border=true&ring=39d353&fire=FF6B35&currStreakLabel=58a6ff&sideLabels=c9d1d9&currStreakNum=c9d1d9&sideNums=c9d1d9&dates=8b949e" />

</div>

---

## 🏆 Contribution Graph — Snake Animation

<!-- Animated snake eating your contributions -->
<div align="center">

<svg width="700" height="250" viewBox="0 0 700 250" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="graphBg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0d1117"/>
      <stop offset="100%" style="stop-color:#161b22"/>
    </linearGradient>
    <filter id="glow2">
      <feGaussianBlur stdDeviation="2" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>
  <rect width="700" height="250" rx="8" fill="url(#graphBg)" stroke="#30363d" stroke-width="1"/>

  <!-- Contribution grid with animated wave pattern -->
  <!-- Row 1 -->
  <g>
    <rect x="20" y="15" width="9" height="9" rx="1" fill="#161b22"/>
    <rect x="33" y="15" width="9" height="9" rx="1" fill="#0e4429"/>
    <rect x="46" y="15" width="9" height="9" rx="1" fill="#006d32"/>
    <rect x="59" y="15" width="9" height="9" rx="1" fill="#26a641"/>
    <rect x="72" y="15" width="9" height="9" rx="1" fill="#39d353"/>
    <rect x="85" y="15" width="9" height="9" rx="1" fill="#26a641"/>
    <rect x="98" y="15" width="9" height="9" rx="1" fill="#0e4429"/>
    <rect x="111" y="15" width="9" height="9" rx="1" fill="#006d32"/>
    <rect x="124" y="15" width="9" height="9" rx="1" fill="#39d353"/>
    <rect x="137" y="15" width="9" height="9" rx="1" fill="#26a641"/>
    <rect x="150" y="15" width="9" height="9" rx="1" fill="#006d32"/>
    <rect x="163" y="15" width="9" height="9" rx="1" fill="#0e4429"/>
    <rect x="176" y="15" width="9" height="9" rx="1" fill="#161b22"/>
    <rect x="189" y="15" width="9" height="9" rx="1" fill="#006d32"/>
    <rect x="202" y="15" width="9" height="9" rx="1" fill="#26a641"/>
    <rect x="215" y="15" width="9" height="9" rx="1" fill="#39d353"/>
    <rect x="228" y="15" width="9" height="9" rx="1" fill="#39d353"/>
    <rect x="241" y="15" width="9" height="9" rx="1" fill="#26a641"/>
    <rect x="254" y="15" width="9" height="9" rx="1" fill="#006d32"/>
    <rect x="267" y="15" width="9" height="9" rx="1" fill="#26a641"/>
    <rect x="280" y="15" width="9" height="9" rx="1" fill="#39d353"/>
    <rect x="293" y="15" width="9" height="9" rx="1" fill="#39d353"/>
    <rect x="306" y="15" width="9" height="9" rx="1" fill="#006d32"/>
    <rect x="319" y="15" width="9" height="9" rx="1" fill="#0e4429"/>
    <rect x="332" y="15" width="9" height="9" rx="1" fill="#26a641"/>
    <rect x="345" y="15" width="9" height="9" rx="1" fill="#39d353"/>
    <rect x="358" y="15" width="9" height="9" rx="1" fill="#006d32"/>
    <rect x="371" y="15" width="9" height="9" rx="1" fill="#0e4429"/>
    <rect x="384" y="15" width="9" height="9" rx="1" fill="#006d32"/>
    <rect x="397" y="15" width="9" height="9" rx="1" fill="#26a641"/>
    <rect x="410" y="15" width="9" height="9" rx="1" fill="#39d353"/>
    <rect x="423" y="15" width="9" height="9" rx="1" fill="#39d353"/>
    <rect x="436" y="15" width="9" height="9" rx="1" fill="#26a641"/>
    <rect x="449" y="15" width="9" height="9" rx="1" fill="#006d32"/>
    <rect x="462" y="15" width="9" height="9" rx="1" fill="#26a641"/>
    <rect x="475" y="15" width="9" height="9" rx="1" fill="#39d353"/>
    <rect x="488" y="15" width="9" height="9" rx="1" fill="#39d353"/>
    <rect x="501" y="15" width="9" height="9" rx="1" fill="#39d353"/>
    <rect x="514" y="15" width="9" height="9" rx="1" fill="#006d32"/>
    <rect x="527" y="15" width="9" height="9" rx="1" fill="#26a641"/>
    <rect x="540" y="15" width="9" height="9" rx="1" fill="#0e4429"/>
    <rect x="553" y="15" width="9" height="9" rx="1" fill="#006d32"/>
    <rect x="566" y="15" width="9" height="9" rx="1" fill="#39d353"/>
    <rect x="579" y="15" width="9" height="9" rx="1" fill="#26a641"/>
    <rect x="592" y="15" width="9" height="9" rx="1" fill="#006d32"/>
    <rect x="605" y="15" width="9" height="9" rx="1" fill="#0e4429"/>
    <rect x="618" y="15" width="9" height="9" rx="1" fill="#26a641"/>
    <rect x="631" y="15" width="9" height="9" rx="1" fill="#39d353"/>
    <rect x="644" y="15" width="9" height="9" rx="1" fill="#006d32"/>
    <rect x="657" y="15" width="9" height="9" rx="1" fill="#26a641"/>
  </g>

  <!-- Rows 2-7 (simplified pattern, filling grid) -->
  <g opacity="0.9">
    <!-- Row 2 -->
    <rect x="20" y="28" width="9" height="9" rx="1" fill="#0e4429"/><rect x="33" y="28" width="9" height="9" rx="1" fill="#26a641"/><rect x="46" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="59" y="28" width="9" height="9" rx="1" fill="#006d32"/><rect x="72" y="28" width="9" height="9" rx="1" fill="#0e4429"/><rect x="85" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="98" y="28" width="9" height="9" rx="1" fill="#26a641"/><rect x="111" y="28" width="9" height="9" rx="1" fill="#006d32"/><rect x="124" y="28" width="9" height="9" rx="1" fill="#0e4429"/><rect x="137" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="150" y="28" width="9" height="9" rx="1" fill="#26a641"/><rect x="163" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="176" y="28" width="9" height="9" rx="1" fill="#006d32"/><rect x="189" y="28" width="9" height="9" rx="1" fill="#0e4429"/><rect x="202" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="215" y="28" width="9" height="9" rx="1" fill="#006d32"/><rect x="228" y="28" width="9" height="9" rx="1" fill="#26a641"/><rect x="241" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="254" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="267" y="28" width="9" height="9" rx="1" fill="#006d32"/><rect x="280" y="28" width="9" height="9" rx="1" fill="#0e4429"/><rect x="293" y="28" width="9" height="9" rx="1" fill="#26a641"/><rect x="306" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="319" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="332" y="28" width="9" height="9" rx="1" fill="#006d32"/><rect x="345" y="28" width="9" height="9" rx="1" fill="#26a641"/><rect x="358" y="28" width="9" height="9" rx="1" fill="#0e4429"/><rect x="371" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="384" y="28" width="9" height="9" rx="1" fill="#26a641"/><rect x="397" y="28" width="9" height="9" rx="1" fill="#006d32"/><rect x="410" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="423" y="28" width="9" height="9" rx="1" fill="#26a641"/><rect x="436" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="449" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="462" y="28" width="9" height="9" rx="1" fill="#006d32"/><rect x="475" y="28" width="9" height="9" rx="1" fill="#0e4429"/><rect x="488" y="28" width="9" height="9" rx="1" fill="#26a641"/><rect x="501" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="514" y="28" width="9" height="9" rx="1" fill="#26a641"/><rect x="527" y="28" width="9" height="9" rx="1" fill="#006d32"/><rect x="540" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="553" y="28" width="9" height="9" rx="1" fill="#0e4429"/><rect x="566" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="579" y="28" width="9" height="9" rx="1" fill="#006d32"/><rect x="592" y="28" width="9" height="9" rx="1" fill="#26a641"/><rect x="605" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="618" y="28" width="9" height="9" rx="1" fill="#006d32"/><rect x="631" y="28" width="9" height="9" rx="1" fill="#0e4429"/><rect x="644" y="28" width="9" height="9" rx="1" fill="#39d353"/><rect x="657" y="28" width="9" height="9" rx="1" fill="#39d353"/>

    <!-- Row 3 -->
    <rect x="20" y="41" width="9" height="9" rx="1" fill="#26a641"/><rect x="33" y="41" width="9" height="9" rx="1" fill="#006d32"/><rect x="46" y="41" width="9" height="9" rx="1" fill="#0e4429"/><rect x="59" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="72" y="41" width="9" height="9" rx="1" fill="#26a641"/><rect x="85" y="41" width="9" height="9" rx="1" fill="#006d32"/><rect x="98" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="111" y="41" width="9" height="9" rx="1" fill="#0e4429"/><rect x="124" y="41" width="9" height="9" rx="1" fill="#26a641"/><rect x="137" y="41" width="9" height="9" rx="1" fill="#006d32"/><rect x="150" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="163" y="41" width="9" height="9" rx="1" fill="#26a641"/><rect x="176" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="189" y="41" width="9" height="9" rx="1" fill="#006d32"/><rect x="202" y="41" width="9" height="9" rx="1" fill="#0e4429"/><rect x="215" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="228" y="41" width="9" height="9" rx="1" fill="#26a641"/><rect x="241" y="41" width="9" height="9" rx="1" fill="#006d32"/><rect x="254" y="41" width="9" height="9" rx="1" fill="#0e4429"/><rect x="267" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="280" y="41" width="9" height="9" rx="1" fill="#26a641"/><rect x="293" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="306" y="41" width="9" height="9" rx="1" fill="#006d32"/><rect x="319" y="41" width="9" height="9" rx="1" fill="#26a641"/><rect x="332" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="345" y="41" width="9" height="9" rx="1" fill="#0e4429"/><rect x="358" y="41" width="9" height="9" rx="1" fill="#006d32"/><rect x="371" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="384" y="41" width="9" height="9" rx="1" fill="#006d32"/><rect x="397" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="410" y="41" width="9" height="9" rx="1" fill="#26a641"/><rect x="423" y="41" width="9" height="9" rx="1" fill="#0e4429"/><rect x="436" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="449" y="41" width="9" height="9" rx="1" fill="#006d32"/><rect x="462" y="41" width="9" height="9" rx="1" fill="#26a641"/><rect x="475" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="488" y="41" width="9" height="9" rx="1" fill="#0e4429"/><rect x="501" y="41" width="9" height="9" rx="1" fill="#26a641"/><rect x="514" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="527" y="41" width="9" height="9" rx="1" fill="#006d32"/><rect x="540" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="553" y="41" width="9" height="9" rx="1" fill="#26a641"/><rect x="566" y="41" width="9" height="9" rx="1" fill="#0e4429"/><rect x="579" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="592" y="41" width="9" height="9" rx="1" fill="#006d32"/><rect x="605" y="41" width="9" height="9" rx="1" fill="#26a641"/><rect x="618" y="41" width="9" height="9" rx="1" fill="#39d353"/><rect x="631" y="41" width="9" height="9" rx="1" fill="#006d32"/><rect x="644" y="41" width="9" height="9" rx="1" fill="#0e4429"/><rect x="657" y="41" width="9" height="9" rx="1" fill="#26a641"/>

    <!-- Row 4 -->
    <rect x="20" y="54" width="9" height="9" rx="1" fill="#006d32"/><rect x="33" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="46" y="54" width="9" height="9" rx="1" fill="#26a641"/><rect x="59" y="54" width="9" height="9" rx="1" fill="#0e4429"/><rect x="72" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="85" y="54" width="9" height="9" rx="1" fill="#006d32"/><rect x="98" y="54" width="9" height="9" rx="1" fill="#26a641"/><rect x="111" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="124" y="54" width="9" height="9" rx="1" fill="#0e4429"/><rect x="137" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="150" y="54" width="9" height="9" rx="1" fill="#006d32"/><rect x="163" y="54" width="9" height="9" rx="1" fill="#26a641"/><rect x="176" y="54" width="9" height="9" rx="1" fill="#006d32"/><rect x="189" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="202" y="54" width="9" height="9" rx="1" fill="#26a641"/><rect x="215" y="54" width="9" height="9" rx="1" fill="#0e4429"/><rect x="228" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="241" y="54" width="9" height="9" rx="1" fill="#006d32"/><rect x="254" y="54" width="9" height="9" rx="1" fill="#26a641"/><rect x="267" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="280" y="54" width="9" height="9" rx="1" fill="#0e4429"/><rect x="293" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="306" y="54" width="9" height="9" rx="1" fill="#26a641"/><rect x="319" y="54" width="9" height="9" rx="1" fill="#006d32"/><rect x="332" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="345" y="54" width="9" height="9" rx="1" fill="#006d32"/><rect x="358" y="54" width="9" height="9" rx="1" fill="#26a641"/><rect x="371" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="384" y="54" width="9" height="9" rx="1" fill="#0e4429"/><rect x="397" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="410" y="54" width="9" height="9" rx="1" fill="#006d32"/><rect x="423" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="436" y="54" width="9" height="9" rx="1" fill="#26a641"/><rect x="449" y="54" width="9" height="9" rx="1" fill="#0e4429"/><rect x="462" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="475" y="54" width="9" height="9" rx="1" fill="#006d32"/><rect x="488" y="54" width="9" height="9" rx="1" fill="#26a641"/><rect x="501" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="514" y="54" width="9" height="9" rx="1" fill="#0e4429"/><rect x="527" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="540" y="54" width="9" height="9" rx="1" fill="#006d32"/><rect x="553" y="54" width="9" height="9" rx="1" fill="#26a641"/><rect x="566" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="579" y="54" width="9" height="9" rx="1" fill="#0e4429"/><rect x="592" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="605" y="54" width="9" height="9" rx="1" fill="#006d32"/><rect x="618" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="631" y="54" width="9" height="9" rx="1" fill="#26a641"/><rect x="644" y="54" width="9" height="9" rx="1" fill="#39d353"/><rect x="657" y="54" width="9" height="9" rx="1" fill="#006d32"/>

    <!-- Row 5 -->
    <rect x="20" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="33" y="67" width="9" height="9" rx="1" fill="#0e4429"/><rect x="46" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="59" y="67" width="9" height="9" rx="1" fill="#26a641"/><rect x="72" y="67" width="9" height="9" rx="1" fill="#006d32"/><rect x="85" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="98" y="67" width="9" height="9" rx="1" fill="#0e4429"/><rect x="111" y="67" width="9" height="9" rx="1" fill="#26a641"/><rect x="124" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="137" y="67" width="9" height="9" rx="1" fill="#006d32"/><rect x="150" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="163" y="67" width="9" height="9" rx="1" fill="#0e4429"/><rect x="176" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="189" y="67" width="9" height="9" rx="1" fill="#26a641"/><rect x="202" y="67" width="9" height="9" rx="1" fill="#006d32"/><rect x="215" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="228" y="67" width="9" height="9" rx="1" fill="#0e4429"/><rect x="241" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="254" y="67" width="9" height="9" rx="1" fill="#26a641"/><rect x="267" y="67" width="9" height="9" rx="1" fill="#006d32"/><rect x="280" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="293" y="67" width="9" height="9" rx="1" fill="#006d32"/><rect x="306" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="319" y="67" width="9" height="9" rx="1" fill="#26a641"/><rect x="332" y="67" width="9" height="9" rx="1" fill="#0e4429"/><rect x="345" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="358" y="67" width="9" height="9" rx="1" fill="#006d32"/><rect x="371" y="67" width="9" height="9" rx="1" fill="#26a641"/><rect x="384" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="397" y="67" width="9" height="9" rx="1" fill="#0e4429"/><rect x="410" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="423" y="67" width="9" height="9" rx="1" fill="#006d32"/><rect x="436" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="449" y="67" width="9" height="9" rx="1" fill="#26a641"/><rect x="462" y="67" width="9" height="9" rx="1" fill="#0e4429"/><rect x="475" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="488" y="67" width="9" height="9" rx="1" fill="#006d32"/><rect x="501" y="67" width="9" height="9" rx="1" fill="#26a641"/><rect x="514" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="527" y="67" width="9" height="9" rx="1" fill="#0e4429"/><rect x="540" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="553" y="67" width="9" height="9" rx="1" fill="#006d32"/><rect x="566" y="67" width="9" height="9" rx="1" fill="#26a641"/><rect x="579" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="592" y="67" width="9" height="9" rx="1" fill="#0e4429"/><rect x="605" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="618" y="67" width="9" height="9" rx="1" fill="#006d32"/><rect x="631" y="67" width="9" height="9" rx="1" fill="#39d353"/><rect x="644" y="67" width="9" height="9" rx="1" fill="#26a641"/><rect x="657" y="67" width="9" height="9" rx="1" fill="#39d353"/>
  </g>

  <!-- Animated scanning line -->
  <rect x="0" y="10" width="3" height="85" rx="1" fill="#58a6ff" opacity="0.4">
    <animate attributeName="x" values="15;670;15" dur="8s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.1;0.5;0.1" dur="8s" repeatCount="indefinite"/>
  </rect>

  <!-- Animated green pulse squares (highlighted contribution cells) -->
  <rect x="280" y="15" width="9" height="9" rx="1" fill="#39d353" filter="url(#glow2)">
    <animate attributeName="opacity" values="0.5;1;0.5" dur="2s" repeatCount="indefinite"/>
  </rect>
  <rect x="488" y="15" width="9" height="9" rx="1" fill="#39d353" filter="url(#glow2)">
    <animate attributeName="opacity" values="0.5;1;0.5" dur="2.5s" repeatCount="indefinite"/>
  </rect>
  <rect x="293" y="28" width="9" height="9" rx="1" fill="#26a641" filter="url(#glow2)">
    <animate attributeName="opacity" values="0.4;1;0.4" dur="3s" repeatCount="indefinite"/>
  </rect>
  <rect x="501" y="54" width="9" height="9" rx="1" fill="#39d353" filter="url(#glow2)">
    <animate attributeName="opacity" values="0.5;1;0.5" dur="2.2s" repeatCount="indefinite"/>
  </rect>

  <!-- Label -->
  <text x="350" y="110" text-anchor="middle" font-family="Segoe UI, Arial, sans-serif" font-size="11" fill="#8b949e">528 contributions in the last year</text>

  <!-- Animated progress bar -->
  <rect x="150" y="125" width="400" height="6" rx="3" fill="#21262d"/>
  <rect x="150" y="125" width="0" height="6" rx="3" fill="#39d353">
    <animate attributeName="width" values="0;340;340" dur="3s" fill="freeze"/>
    <animate attributeName="opacity" values="0.6;1;0.8" dur="2s" repeatCount="indefinite"/>
  </rect>
  <text x="560" y="133" font-family="JetBrains Mono, monospace" font-size="10" fill="#39d353">
    <animate attributeName="opacity" values="0;1;1" dur="3s" fill="freeze"/>
    85%
  </text>

  <!-- Animated fire particles rising from contribution cells -->
  <circle cx="280" cy="15" r="2" fill="#f7c948" opacity="0">
    <animate attributeName="cy" values="15;-20;-60" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.8;0.4;0" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="r" values="2;1;0" dur="3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="488" cy="15" r="2" fill="#f7c948" opacity="0">
    <animate attributeName="cy" values="15;-25;-65" dur="3.5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.8;0.4;0" dur="3.5s" repeatCount="indefinite"/>
    <animate attributeName="r" values="2;1.5;0" dur="3.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="124" cy="15" r="1.5" fill="#ff6b35" opacity="0">
    <animate attributeName="cy" values="15;-15;-50" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;0.3;0" dur="4s" repeatCount="indefinite"/>
  </circle>

</svg>

</div>

---

<div align="center">

<svg width="700" height="30" viewBox="0 0 700 30" xmlns="http://www.w3.org/2000/svg">
  <line x1="0" y1="15" x2="700" y2="15" stroke="#30363d" stroke-width="0.5"/>
  <circle cx="50" cy="15" r="3" fill="#f78166">
    <animate attributeName="cx" values="50;350;650;350;50" dur="6s" repeatCount="indefinite"/>
    <animate attributeName="r" values="2;5;3;4;2" dur="6s" repeatCount="indefinite"/>
  </circle>
  <circle cx="650" cy="15" r="3" fill="#58a6ff">
    <animate attributeName="cx" values="650;350;50;350;650" dur="6s" repeatCount="indefinite"/>
    <animate attributeName="r" values="3;5;2;4;3" dur="6s" repeatCount="indefinite"/>
  </circle>
</svg>

</div>

## 🏆 Trophies

<div align="center">

[![trophy](https://github-profile-trophy.vercel.app/?username=Rohit7696&theme=algolia&no-frame=true&no-bg=true&column=7&margin-w=10)](https://github.com/ryo-ma/github-profile-trophy)

</div>

---

## 🐍 Contribution Snake

<!-- If you set up the snake animation workflow -->
<!-- Replace this with your actual snake gif URL after setup -->

<div align="center">

[![Snake animation](https://raw.githubusercontent.com/Rohit7696/Rohit7696/output/github-contribution-grid-snake-dark.svg)](https://raw.githubusercontent.com/Rohit7696/Rohit7696/output/github-contribution-grid-snake-dark.svg)

</div>

---

<div align="center">

<svg width="700" height="30" viewBox="0 0 700 30" xmlns="http://www.w3.org/2000/svg">
  <line x1="0" y1="15" x2="700" y2="15" stroke="#30363d" stroke-width="0.5"/>
  <circle cx="350" cy="15" r="4" fill="#d2a8ff" filter="url(#glow2)">
    <animate attributeName="r" values="3;6;3" dur="2s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.5;1;0.5" dur="2s" repeatCount="indefinite"/>
  </circle>
</svg>

</div>

## 🎯 Current Focus

---

## 📈 Profile Visitors

<div align="center">

[![Visitors](https://visitcount.itsvg.in/api?id=Rohit7696&icon=2&color=6)](https://visitcount.itsvg.in)

</div>

---

<div align="center">

<svg width="700" height="80" viewBox="0 0 700 80" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="footerGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#58a6ff"/>
      <stop offset="50%" style="stop-color:#f78166"/>
      <stop offset="100%" style="stop-color:#d2a8ff"/>
    </linearGradient>
  </defs>

  <!-- Animated footer line -->
  <line x1="50" y1="30" x2="650" y2="30" stroke="url(#footerGrad)" stroke-width="1" stroke-dasharray="5,5">
    <animate attributeName="stroke-dashoffset" values="0;-20" dur="2s" repeatCount="indefinite"/>
  </line>

  <!-- Pulsing center dot -->
  <circle cx="350" cy="30" r="4" fill="#58a6ff">
    <animate attributeName="r" values="3;6;3" dur="2s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;1;0.6" dur="2s" repeatCount="indefinite"/>
  </circle>

  <!-- Footer text -->
  <text x="350" y="60" text-anchor="middle" font-family="JetBrains Mono, monospace" font-size="10" fill="#484f58">
    "Consistency beats intensity. Show up every day."
  </text>

  <!-- Running dots -->
  <circle cx="0" cy="30" r="2" fill="#39d353" opacity="0.6">
    <animate attributeName="cx" values="50;350;650" dur="6s" repeatCount="indefinite"/>
  </circle>
  <circle cx="700" cy="30" r="2" fill="#f78166" opacity="0.6">
    <animate attributeName="cx" values="650;350;50" dur="6s" repeatCount="indefinite"/>
  </circle>
</svg>

</div>

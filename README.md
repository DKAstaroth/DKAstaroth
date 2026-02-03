<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0d1117,161b22,0d1117&height=320&section=header&text=JUAN%20PABLO%20VEGA&fontSize=70&fontColor=c9d1d9&animation=fadeIn&fontAlignY=38&desc=Building%20Scalable%20Systems%20%7C%20Engineering%20Excellence&descAlignY=55&descAlign=50" alt="Master Header" width="100%" />
</div>

<h3 align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=25&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&width=600&lines=Software+Engineer;Complex+Problem+Solver;System+Architect;Python+%2B+Cloud+Specialist" alt="Typing SVG" />
  </a>
</h3>

<div align="center">
  <a href="https://linkedin.com/in/vega-core">
    <img src="https://img.shields.io/badge/LINKEDIN-CONNECT-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:vegalagos.jpa@gmail.com">
    <img src="https://img.shields.io/badge/EMAIL-SEND_MESSAGE-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://github.com/DKAstaroth">
    <img src="https://img.shields.io/badge/GITHUB-REPO_ACCESS-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
</div>

<br />

<div align="center">
  <blockquote>
    <i>"La diferencia entre código funcional y código excelente radica en la escalabilidad, la legibilidad y la arquitectura subyacente."</i>
  </blockquote>
</div>

<br />

<h2 align="center">📊 Engineering Analytics & Activity</h2>

<div align="center">
  <a href="https://github.com/ryo-ma/github-profile-trophy">
    <img src="https://github-profile-trophy.vercel.app/?username=DKAstaroth&theme=gitdimmed&no-frame=true&no-bg=true&margin-w=4" alt="DKAstaroth Trophies" />
  </a>
</div>

<br>

<table align="center" width="95%" style="border: none;">
  <tr>
    <td width="55%" align="center" style="border: none;">
      <img src="https://github-readme-stats.vercel.app/api?username=DKAstaroth&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=58A6FF&icon_color=c9d1d9&count_private=true" alt="Juan Pablo's GitHub Stats" width="100%" />
    </td>
    <td width="45%" align="center" style="border: none;">
      <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=DKAstaroth&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=58A6FF&text_color=c9d1d9&langs_count=6" alt="Top Languages" width="100%" />
    </td>
  </tr>
</table>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=DKAstaroth&theme=tokyonight&hide_border=true&background=0d1117&ring=58A6FF&fire=D14836&currStreakLabel=58A6FF" alt="GitHub Streak" />
</div>

<br />
<hr>

## ⚡ Tech Stack & Ecosystem

<table align="center">
  <tr>
    <td align="center" width="120">
      <img src="https://techstack-generator.vercel.app/python-icon.svg" alt="icon" width="55" height="55" />
      <br><b>Core Logic</b>
    </td>
    <td align="center" width="120">
      <img src="https://techstack-generator.vercel.app/ts-icon.svg" alt="icon" width="55" height="55" />
      <br><b>Typed Stack</b>
    </td>
    <td align="center" width="120">
      <img src="https://techstack-generator.vercel.app/docker-icon.svg" alt="icon" width="55" height="55" />
      <br><b>Containerization</b>
    </td>
    <td align="center" width="120">
      <img src="https://techstack-generator.vercel.app/mysql-icon.svg" alt="icon" width="55" height="55" />
      <br><b>Persistence</b>
    </td>
    <td align="center" width="120">
      <img src="https://techstack-generator.vercel.app/aws-icon.svg" alt="icon" width="55" height="55" />
      <br><b>Cloud Infra</b>
    </td>
    <td align="center" width="120">
      <img src="https://user-images.githubusercontent.com/25181517/192108372-f71d70ac-7ae6-4c0d-8395-5190795500d3.png" alt="icon" width="55" height="55" />
      <br><b>Git Flow</b>
    </td>
  </tr>
</table>

<br />

---

## 📐 System Architecture Review

<details open>
<summary><b>CASE STUDY I: High-Availability Resource Orchestration (S.G.R.E)</b></summary>
<br>
  
> **Concept:** Sistema distribuido para logística de emergencia con *throttling* inteligente de notificaciones.
> **Challenge:** Manejar concurrencia en escritura y garantizar entrega de alertas sin saturar el canal.

```mermaid
graph TD
    subgraph "Core Infrastructure"
    LB[Load Balancer] --> API[API Gateway]
    API --> AUTH{Auth Service}
    end

    subgraph "Logic Layer"
    AUTH -- Valid --> ENGINE[JSON Logic Engine]
    ENGINE --> QUEUE[(Redis/Job Queue)]
    end

    subgraph "Persistence & Async"
    QUEUE -- Dequeue --> WORKER[Background Worker]
    WORKER --> DB[(NoSQL Cluster)]
    WORKER --> NOTIFY[Notification Service]
    end

    style ENGINE fill:#2ea44f,stroke:#fff,stroke-width:2px,color:#fff
    style QUEUE fill:#db6d28,stroke:#fff,stroke-width:2px,color:#fff
    style DB fill:#1f6feb,stroke:#fff,stroke-width:2px,color:#fff

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0f172a&height=280&section=header&text=JUAN%20PABLO%20VEGA&fontSize=80&animation=fadeIn&fontAlignY=35&desc=Automated%20Solutions%20Architect%20%7C%20Cloud%20Engineer&descAlignY=55&descAlign=50" alt="Header Architect" width="100%" />
</div>

<h3 align="center">
  <code>Input: Complex Problems</code> ➔ <code>Process: System Architecture</code> ➔ <code>Output: Scalable Solutions</code>
</h3>

<div align="center">
  <a href="https://linkedin.com/in/vega-core">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin" alt="LinkedIn" />
  </a>
  <a href="mailto:vegalagos.jpa@gmail.com">
    <img src="https://img.shields.io/badge/Email-Contact_Me-EA4335?style=for-the-badge&logo=gmail" alt="Email" />
  </a>
  <a href="https://github.com/DKAstaroth">
    <img src="https://img.shields.io/badge/GitHub-Profile-181717?style=for-the-badge&logo=github" alt="GitHub" />
  </a>
</div>

<br />

---

## 🏗️ Ingeniería & Arquitectura
> *"La excelencia técnica no es un acto, es un hábito metódico."*

Soy un **Arquitecto de Soluciones Automatizadas** especializado en el diseño de ecosistemas digitales resilientes. Mi enfoque combina la lógica estricta de la ingeniería de software con la flexibilidad de las arquitecturas Cloud Native.

| Dominio | Competencias Clave |
| :--- | :--- |
| **Cloud Infrastructure** | Huawei Cloud (ECS, VPC, ELB), AWS, Arquitecturas Serverless. |
| **Backend Logic** | Python (Advanced), Node.js, JSON Logic Processing, Asynchronous Queues. |
| **Data Engineering** | SQL Optimization, NoSQL Modeling (Document-based), ETL Pipelines. |
| **Automation** | CI/CD Flows, Process Orchestration, MasterBase Smartview. |

<br />

## 🛠️ Stack Tecnológico (Nivel Producción)

<div align="center">
  <table>
    <tr>
      <td align="center" width="90">
        <img src="https://skillicons.dev/icons?i=python" width="45" height="45" alt="Python" />
        <br>Python
      </td>
      <td align="center" width="90">
        <img src="https://skillicons.dev/icons?i=ts" width="45" height="45" alt="TypeScript" />
        <br>TypeScript
      </td>
      <td align="center" width="90">
        <img src="https://skillicons.dev/icons?i=docker" width="45" height="45" alt="Docker" />
        <br>Docker
      </td>
      <td align="center" width="90">
        <img src="https://skillicons.dev/icons?i=linux" width="45" height="45" alt="Linux" />
        <br>Linux
      </td>
      <td align="center" width="90">
        <img src="https://skillicons.dev/icons?i=postgres" width="45" height="45" alt="PostgreSQL" />
        <br>SQL
      </td>
      <td align="center" width="90">
        <img src="https://skillicons.dev/icons?i=git" width="45" height="45" alt="Git" />
        <br>Git Flow
      </td>
      <td align="center" width="90">
        <img src="https://skillicons.dev/icons?i=huawei" width="45" height="45" alt="Huawei" />
        <br>Huawei Cloud
      </td>
    </tr>
  </table>
</div>

<br />

---

## 🧬 Proyectos & Diseño de Sistemas
*A continuación se presentan diagramas de alto nivel de mis desarrollos más complejos.*

<details open>
<summary><h3>🚨 S.G.R.E. - Sistema de Gestión de Recursos de Emergencia</h3></summary>
<br>

**Rol:** Lead Architect & Developer | **Stack:** NoSQL, JSON Logic, Distributed Scheduling.

> Plataforma logística crítica diseñada para alta disponibilidad y orquestación compleja de recursos bajo demanda.

```mermaid
graph LR
    subgraph Client_Side
    UI[Frontend Interface] -->|JSON Request| API[API Gateway]
    end

    subgraph Core_Logic
    API -->|Validate| JL[JSON Logic Engine]
    JL -->|Process Rules| CTRL[Controller]
    end

    subgraph Data_Persistence
    CTRL -->|Write/Read| DB[(NoSQL Heterogeneous DB)]
    end

    subgraph Async_Worker
    CTRL -->|Enqueue Job| Q[Scheduling Queue]
    Q -->|Trigger Interval| NOTIF[Notification Service]
    NOTIF -->|Render HTML/CSS| EMAIL[Dynamic Report Dispatch]
    end

    style API fill:#f9f,stroke:#333,stroke-width:2px
    style DB fill:#bbf,stroke:#333,stroke-width:2px
    style JL fill:#bfb,stroke:#333,stroke-width:2px

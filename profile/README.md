# Learning Dashboard

Tool to visualize and monitor the achievement of learning objectives in subjects based on the development of team software projects.

The system captures events from GitHub, Taiga and Google Sheets, processes them into metrics and quality indicators, and presents them via a web dashboard and administration tool.

## Repositories

To deploy the system: **[learning-dashboard-deploy](https://github.com/Learning-Dashboard/learning-dashboard-deploy)** (Docker Compose + submodules).

### Main submodules

| Repository | What it does | Tech |
|---|---|---|
| [LD-learning-dashboard](https://github.com/Learning-Dashboard/LD-learning-dashboard) | Main application (dashboard, predictions, simulations) | Java, Spring Boot, AngularJS |
| [LD_Connect_Event](https://github.com/Learning-Dashboard/LD_Connect_Event) | Ingestió d'esdeveniments (webhooks GitHub/Taiga/Sheets → MongoDB) | Python, Flask |
| [LD_Eval_Event](https://github.com/Learning-Dashboard/LD_Eval_Event) | Recalculation of quality metrics and indicators | Python, Flask |
| [LD_admintool_frontend](https://github.com/Learning-Dashboard/LD_admintool_frontend) | Frontend of the administration tool | React, Vite |
| [LD_admintool](https://github.com/Learning-Dashboard/LD_admintool) | Administration tool backend (teams, projects, Excel imports) | Java, Spring Boot 3 |

## Bug Reporting

All bugs should be reported here:
[https://github.com/Learning-Dashboard/Bug-Reporting](https://github.com/Learning-Dashboard/Bug-Reporting)

- Create a "Bug Report" type issue with a clear description, steps to reproduce and evidence (logs/captures)
- Indicate the related components (dashboard, connect, eval, admintool…)

Please, do not open bugs in concrete code repositories
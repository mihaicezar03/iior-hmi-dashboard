# Industrial HMI Dashboard | IIOR University Project

**Role-Based Human–Machine Interface Prototype for an Automated Production Line**  
University coursework · Industrial Automation · HMI Design  
**Author:** Mihai-Cezar Moldovan

## Overview

A browser-based **Human–Machine Interface (HMI) prototype** designed to explore monitoring, control, and decision-support interfaces for a robotized production environment. The project combines requirements analysis, user-role definitions, interface wireframes, and a navigable set of dashboards for production stakeholders.

The prototype is presented under the fictional **Becks & Decker** concept. The accompanying academic report describes a **chess-set handling, inspection, packaging, and palletizing** production-line scenario. It is a frontend demonstration, **not a deployment connected to PLCs, industrial robots, or live manufacturing data**.

## Key features

- **Role-specific dashboards:** Operator, Process Engineer, Quality Control Engineer, Maintenance Engineer, and Manager.
- **Operator interface:** Start, Stop and Reset controls, production counts, logs, and status indicators represented in the UI.
- **Process engineering:** Throughput charts, cycle-time metrics, setup history, and bottleneck-identification panels.
- **Quality control:** Inspection summaries, defect categories, traceability information, and sampling-plan status.
- **Maintenance:** Cycle counters, alarm history, diagnostics, spare-part inventory, and maintenance information.
- **Management:** Production summaries, equipment effectiveness, energy usage, downtime, and shift comparison.
- **Navigation:** Consistent menu layout, separate dashboard pages, and simulated role-based access.

## Technology

| Area | Components / tools |
| --- | --- |
| Frontend | HTML, CSS, client-side JavaScript |
| Structure | Multiple role-specific dashboard pages |
| Login demonstration | Client-side role selection and local browser storage |
| Interface design | Wireframes, information hierarchy, and industrial HMI conventions |
| Requirements | Stakeholder analysis, use cases, usability criteria, and performance characteristics |

## Run locally

1. Download or clone the repository.
2. Open `website/index.html` in a web browser; the main interface is also accessible via `website/home.html`.
3. Navigate to the login page to explore the role-based dashboards. See the on-screen demonstration login hints.

**Security note:** The supplied login uses a shared demonstration password and checks roles in browser-side JavaScript. It is **not secure authentication** and should not be reused for a production application. Dashboard values are illustrative; buttons and panels do not control actual machinery.

## Project structure

```text
iior-hmi-dashboard/
├── README.md
└── website/
    ├── index.html
    ├── home.html
    ├── login.html
    ├── dashboard-operator.html
    ├── dashboard-process.html
    ├── dashboard-qa.html
    ├── dashboard-maintenance.html
    ├── dashboard-manager.html
    ├── styles.css
    └── images/
```

## Design process

The project report documents stakeholder needs, functional and non-functional requirements, a requirements/performance relationship matrix, use-case definitions, interface wireframes, technology selection, and a usability evaluation. The design emphasizes making relevant information accessible to each operational role without overloading other users.

## Limitations and future improvements

- **No industrial control integration:** No verified connection to a PLC, HMI panel, field devices, or real manufacturing data.
- **Demonstration authentication:** Browser-side checks are not a security boundary.
- **Illustrative data:** The interface does not establish real production throughput, uptime, or alarm-response performance.
- **Next steps:** Implement secure server-side authentication, live data acquisition, alarm acknowledgement persistence, responsive layouts, and structured usability testing with operators.

## Academic context

Developed as an **IIOR university project** exploring the design of a multi-role industrial HMI. This public repository shares the prototype code and a concise overview rather than the complete course report and submission archive.

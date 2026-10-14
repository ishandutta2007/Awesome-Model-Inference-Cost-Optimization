# Awesome-Model-Inference-Cost-Optimization

## Top Modernized Metal Mill Operations Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Metallurgical Process Optimization, Quality Execution & Plant-Scale AI Monitoring*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Modernized Metal Mill Operations**. These tools optimize metallurgical heat settings, track quality through the full production chain from melt shop to finished coil, and provide plant-scale AI monitoring to prevent unplanned downtime and surface defects.

**Examples** include Quinlogic (SMS group), PSI Metals, Primetals Technologies, TMEIC, Falkonry, SmartSteel, Tenova, Fives Group, Danieli Automation, and ANDRITZ Metals (the category leaders).

**Open-source emphasis**: This section is expanded with the most relevant open-source projects for metal mill operations — production planning, MES, and simulation — ideal for plant engineers prioritizing data sovereignty, developers building industrial pipelines, and teams avoiding per-seat proprietary licensing.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Quinlogic (SMS group)](https://www.quinlogic.com/)**  
  Quality Execution System (QES) that analyzes online process, production, and quality data from steelmaking through casting, rolling, and drawing. The **DataCorrelator** module applies big data analysis and AI to identify quality-relevant patterns across isolated production lines [citation:1][citation:16]. Features **LogicDesigner** for flexible rule customization, automatic product grading, surface defect mapping, and digital twin representation of each coil [citation:16]. Deployed at Swiss Steel's Emmenbrücke plant for group-wide Industry 4.0 initiative [citation:6].

- **[PSI Metals (PSImetals)](https://www.psi.de/en/solutions/products/psimetals)**  
  Integrated production management platform combining Supply Chain Management, Advanced Planning & Scheduling, and Manufacturing Execution System with **Quality and Order Dressing** [citation:7][citation:17]. Supports end-to-end processes from melt shop to shipping with continuous material genealogy and production history [citation:17]. Implemented at **Tata Steel Nederland** (IJmuiden) for heat and slab qualification, reducing incorrect material production and supporting Green Steel sustainability goals [citation:2]. Strategic partnership with **qoncept** adds **qontrol maps** for real-time scrap quality assessment and automated charge mix optimization for EAF and BOF processes [citation:12]. Java-based, on-premises or cloud, certified SAP integration [citation:7].

- **[Falkonry](https://www.falkonry.com/)**  
  Time Series AI platform for automated anomaly detection and diagnosis at plant scale. Detects precursor conditions to equipment failures **3-10 weeks in advance** without requiring data scientists or ML engineers [citation:13]. Monitors hundreds of motors and couplers simultaneously in real time, identifying signal conditions that introduce surface defects [citation:8]. Integrated with **iba** high-speed data acquisition for Parquet-based ingestion — processes 180,000 rows across ~200 signals in **~2 minutes** [citation:18]. Documented results: **$285,750 prevented loss per incident** and **~$4.5M/yr productivity increase** at a North American steel manufacturer [citation:8].

- **[Primetals Technologies](https://www.primetals.com/)**  
  Metallurgical plant engineering and automation with process optimization, digitalization, and quality management for steel mills.

- **[TMEIC](https://www.tmeic.com/)**  
  Industrial automation and drive systems for metals with process control, quality monitoring, and production optimization.

- **[SmartSteel](https://www.smartsteel.com/)**  
  Digital solutions for steel production with process optimization and quality management.

- **[Tenova](https://www.tenova.com/)**  
  Metals industry equipment and automation with process control and digital solutions.

- **[Fives Group](https://www.fivesgroup.com/)**  
  Industrial engineering with automation and process control for metals production.

- **[Danieli Automation](https://www.danieli.com/)**  
  Automation and process control systems for steelmaking, rolling, and finishing.

- **[ANDRITZ Metals](https://www.andritz.com/)**  
  Metals processing equipment with automation and digital solutions for quality and efficiency.

## Open-Source GitHub Projects

- **[DynReAct](https://github.com/DynReAct/OSS_Platform)**  
  **Open-source production planning platform for the steel sector** developed under EU RFCS Grant Agreement No 101112421 [citation:4][citation:14]. Implements **hierarchical planning across three levels**: Long-Term Planning (LTP, monthly targets), Mid-Term Planning (MTP, lot creation and order scheduling), and Short-Term Planning (STP, intra-day deviations via Multi-Agent System) [citation:4]. Features **Plant Performance Models (PPMs)** — independent services with standard interfaces that query feasibility of producing orders at given plants and propose alternative schedules [citation:4]. Uses **Genetic Algorithms** for coil allocation and **Fuzzy Inference System** for simulating human decision-making in allocation criteria [citation:14]. Sample scenario and template PPM included for customization via Python plugin interface. Beta release planned mid-2025, technical specification in 2026 [citation:4].

- **[OpenMES](https://github.com/Mes-Open/OpenMes)**  
  **Open-source Manufacturing Execution System** shaped through consultations with manufacturing companies across industries [citation:5]. Features **hook-based architecture** with `ResourceChanged` CRUD hooks for work orders/customers/materials/lines, `WorkOrderScheduled` events, `MenuRegistry` for sidebar additions, and `WidgetRegistry` for dashboard cards [citation:5]. Built-in **Packaging module** with EAN barcode scanning station, scan history logging, shift-based counters, and live stats updating every 3 seconds [citation:5]. Laravel 12 + Tailwind CSS 4 + Alpine.js + Livewire 4 stack. Supports ERP integration (SAP, Odoo), IoT integration, quality control automation, and custom reporting [citation:5].

- **[WebErpMesv2](https://github.com/SMEWebify/WebErpMesv2)**  
  **Free, open-source ERP and MES for small industry** (sheet metal, machining, molds) under MIT license [citation:10][citation:20]. Runs the full quote-to-delivery flow: commercial pipeline, sales orders, production planning and shop-floor execution, stock and purchasing, and **ISO 9001 quality management** [citation:20]. Laravel 12 + PHP 8.3 + MariaDB stack, deployable on Ubuntu 24.04 via Microsoft Marketplace with no per-seat fees [citation:20]. 220+ GitHub stars, 21 releases, 85+ PHPUnit test files [citation:10].

- **[Steel Industry Digital Twin](https://github.com/marcosoares-92/steelindustrysimulator)**  
  **Google Colab-based simulator** reproducing energy consumption behavior of a small-scale steel facility (DAEWOO Steel Co. Ltd, Gwangyang, South Korea) [citation:19]. Uses deep learning to model plant operation parameters including lagging/leading reactive power, CO2 ppm, and load type (Light/Medium/Maximum) [citation:19]. Goal: **minimize energy consumption in kWh** through parameter optimization. Based on UCI Steel Industry Energy Consumption Dataset [citation:19].

- **[JaamSim Steel Plant Simulation](https://jaamsim.com/)**  
  Open-source discrete-event simulation software used for **energy efficiency and productivity analysis** in a Brazilian steel plant [citation:9]. Enables scenario modeling and bottleneck identification without proprietary simulation licensing.

### Additional Strong Open-Source Options

- **qcadoo MES** — Open-source MES for manufacturing with production management, work orders, and shop-floor control. 809+ GitHub stars [citation:15].
- **ERPNext** — Full open-source ERP with manufacturing modules adaptable for metal production planning and inventory.
- **Odoo Manufacturing** — Open-source ERP with MRP, work centers, and quality control modules.
- **freePPLE** — Open-source supply chain planning for production and inventory optimization. 535+ GitHub stars [citation:15].
- **Apache PLC4X** — Universal protocol adapter for industrial PLCs (Modbus, OPC UA, Siemens S7) for plant data ingestion.
- **InfluxDB + Grafana** — Open-source time-series database and visualization stack for custom mill monitoring dashboards.

**Frameworks for building custom systems**: Combine **DynReAct** for hierarchical production planning with multi-agent short-term scheduling, **OpenMES** or **WebErpMesv2** for shop-floor execution and quality management, **Steel Industry Digital Twin** for energy simulation, and **Apache PLC4X + InfluxDB + Grafana** for plant data ingestion and visualization to build a complete self-hosted metal mill operations stack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Metal mill operations platforms must comply with industrial safety standards, environmental regulations, and quality certifications (ISO 9001, IATF 16949). **Metallurgical heat settings and process optimizations must be validated by qualified metallurgists before implementation** — incorrect parameters can cause equipment damage, safety hazards, or material downgrades.
- Self-hosted open-source solutions require proper industrial network integration, OT/IT security hardening, and domain expertise for configuration and validation.

---

**Made for metallurgical engineers, plant managers, process control specialists, and developers building steel mill optimization platforms.**  
Let's make modernized metal mill operations more open, data-driven, and quality-focused.

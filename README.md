<h1 align="center">Engr. Muhammad Fahad</h1>
<p align="center"><b>Electrical Power Engineer | Transmission & Utilities | Embedded Systems</b><br>
PEC Registered Engineer · Pakistan (Islamabad)<br>
📧 engrfahad114259@gmail.com</p>

---

# 💫 About Me

I'm an Electrical Power Engineer (BEngg., UET Peshawar, PEC accredited Washington Accord) who works across two worlds: **power systems and utilities** (substation design, SLDs, protection, load flow, field work on LESCO and PESCO networks) and **embedded systems** (bare-metal firmware, PCB design, smart energy metering). I like work that goes from a drawing or a datasheet all the way to a device running in the field.

🔧 **I'm currently working on**<br>
Open source fixes for grid software (OpenSTEF, Grid2Op, OpenLEADR), bare-metal firmware for MIPS32 M4K (PIC32) microcontrollers through direct register manipulation, ISRs and peripheral control, and projects on load forecasting and fault classification.

🤝 **I'm looking to collaborate on**<br>
Power and utilities projects (drawings, studies, documentation), open source grid and energy tools, RTOS development, low level hardware programming without HAL, and custom PCB debugging.

🌍 **I'm open to**<br>
Remote internships and volunteer work with power, utilities and grid teams. I'm happy to take on daily engineering tasks such as SLDs and drawings in AutoCAD or EPLAN, ETAP studies, data sheets, reports and weekly updates, so senior engineers can focus on the main work.

🆘 **I'm looking for help with**<br>
Advanced MIPS assembly optimizations and timing critical ISRs for hardware interfaces.

📚 **I'm currently learning**<br>
Grid simulation and demand response software, time series load forecasting, PIC32 architecture documentation, DMA register configuration and silicon errata mitigation.

💬 **Ask me about**<br>
Substation SLDs, ETAP load flow, PIC/STM/AVR register programming, DLMS/COSEM smart metering, bit-banging protocols, or why 7 hours of debugging can save you from 4 minutes of reading documentation 😉

---

# 💼 Experience

### Jr. Field Engineer, CISNR (Center for Intelligent Systems and Network Research), UET Peshawar
*July 2025 – Oct 2026*
- Developed bare-metal firmware for a smart energy meter on a PIC32 microcontroller for the German BMZ funded **GIZ DDPG** project, enabling real time acquisition of grid power quality data.
- Led a field survey across 31 transformer feeders to set a baseline for load and power quality studies, in partnership with GIZ GmbH Pakistan. Led a survey of the 132/11 kV Saidpur Feeder at LESCO (transformer and pole level data, user counts per pole, GPS coordinates).
- Deployed and commissioned a network of 155 monitoring devices (8 at transformers, 147 at consumer points covering 1400 users) for real time grid performance analysis.
- Led the LESCO installation team for 180+ Electrocure devices and supervised a LESCO maintenance team troubleshooting offline devices. Supported the APMS installation at PESCO.
- Tested 200+ Electrocure, 30+ Transfocure and 5+ APMS units, fixing circuit, PCB and firmware faults, and built test automation tools to cut manual effort.
- Managed field reports, records and QA/QC documentation for installed devices; monitored and maintained 135 WaterSCADA tubewell monitoring and protection devices (WSSP Peshawar).
- Assisted the commissioning team in preparing APMS for PPMC licensing: sensor integration, DLMS/COSEM support, MCCB/MCC schemes, panel and enclosure design.

### Trainee Engineer (Remote), Techno Engineering Services Pvt Ltd
*Feb 2026 – June 2026*
- Prepared single line diagrams (SLDs) and diagrams for a 132 kV grid station in AutoCAD, plus substation layouts and schemes.
- Made panel drawings in EPLAN and used ETAP on project based power system work.

### Electrical Engineer Intern, WAPDA Chashma Hydel Power Station (O&M Electrical Section)
*July 2024 – Sep 2024*
- Assisted in monitoring 184 MW turbine generators and in preventive maintenance of AVR/exciter systems (97% reliability).
- Supported troubleshooting of 132 kV transformer and generator faults and debugged a faulty SCADA system controlling shaft blade angles and flow rate.

### Project Engineer (Intern) and STEM Instructor, Rduinotronics (R&D Section), Peshawar
- Designed 10+ embedded system PCBs, reducing integration time by 25%.
- Reverse engineered UPS systems, reaching 80% load stability in prototype testing.
- Taught PCB design as a STEM instructor and contributed to project development at the startup.

---

# 🌐 Open Source Contributions

### [OpenSTEF](https://github.com/OpenSTEF/openstef) (Alliander and LF Energy): learning curve visualization, PR [#1183](https://github.com/OpenSTEF/openstef/pull/1183)
- Added a `LearningCurveMixin`, a table builder and an interactive Plotly chart that shows whether a forecasting model is overfitting, with support in the XGBoost and GBLinear forecasters.
- 19 unit tests and a new tutorial section (12 files, +561 lines). Checked on the real Liander dataset and followed the project's rules (Conventional Commits, MPL-2.0 headers, DCO sign off, lint and type checks).
- Found a separate bug (`eval_set` is not passed to LightGBM base learners) and kept it for a second pull request.

### [Grid2Op](https://github.com/Grid2op/grid2op) (LF Energy): load injection dispatch fix, issue #777, PR [#790](https://github.com/Grid2op/grid2op/pull/790)
- Fixed a bug where load changes made by an action were never declared to the redispatch, so the slack generator silently exceeded its pmax and ramp limits. Generators now share the change within limits, or the episode ends with `ImpossibleRedispatching`.
- New `LoadInjectionModule`, 14 regression tests (3 main tests fail when the fix is removed), changelog entry (9 files, +336 lines). My own test caught a first design mistake and I reworked it.

### [OpenLEADR](https://github.com/OpenLEADR/openleadr-python) (OpenADR 2.0b demand response): single completed event fix, issue #175
- Found the root cause of an empty event list sent to a polling VEN: for one event, the response and the queue were the same Python list. Fix: build the response from a copy.
- 4 new tests including a full VTN and VEN test (2 files, +93 lines); 2 of the new tests fail without the fix; full suite passed.

---

# 🔬 Research and Publications

- **Prespecified Memorization Test for Zero Shot Load Forecasting with Foundation Models**. Muhammad F., Niaz M. K., Ahad A., Arsalan A. M., Syed A. S. *Submitted to the 7th International Conference on Innovative Computing (ICIC), IEEE.*
- **Placebo Calibrated Out of Time Evaluation of Zero Shot Foundation Models for Grid Load**. Muhammad F., Niaz M. K., Ahad A., Arsalan A. M., Syed A. S. *Submitted to the 7th International Conference on Innovative Computing (ICIC), IEEE.*
- **Time Surface Encoded Spiking Neural Networks for Transmission Line Fault Classification on Noisy Memristive Crossbars**. Niaz M. K., Muhammad F., Ahad A. *Published in the 2nd International Conference on Evolution of Artificial Intelligence (ICEAI), HEC IJIST Y Category Journal.*

**Ongoing research:**
- Multi component fault diagnosis in HTGR helium Brayton cycles
- Fault localization with sparse or limited PMU coverage
- Impact of converter current limiting and prioritization strategies on protection in IBR heavy, HVDC connected grids
- System 1.5: familiarity gated cognition for self aware machine intelligence

---

# 🛠️ Independent Projects

- **Smart Energy Meter with fault protection**
- **Wireless Power Transfer based EV charging station and monitoring**
- **DodgeGoku** (ESP32, MPU6050, FreeRTOS)
- **Battery Management System (SoC estimation):** regression based State of Charge algorithm validated against real discharge cycles, with HC-SR04.

---

# 🎓 Education

**BEngg. in Electrical Power Engineering**, University of Engineering and Technology (UET) Peshawar, Nov 2021 – Oct 2025. CGPA 3.08/4.00. Accredited by the Pakistan Engineering Council (PEC) Washington Accord.

---

# 💻 Tech Stack and Skills

![C](https://img.shields.io/badge/c-%2300599C.svg?style=flat&logo=c&logoColor=white) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=flat&logo=c%2B%2B&logoColor=white) ![Python](https://img.shields.io/badge/python-3776AB?style=flat&logo=python&logoColor=white) ![MATLAB](https://img.shields.io/badge/MATLAB-Simulink-0076A8?style=flat) ![R](https://img.shields.io/badge/R-276DC3?style=flat&logo=r&logoColor=white) ![Arduino](https://img.shields.io/badge/-Arduino-00979D?style=flat&logo=Arduino&logoColor=white) ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=flat&logo=github&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=flat&logo=amazon-aws&logoColor=white) ![ETAP](https://img.shields.io/badge/ETAP-1F3864?style=flat) ![PSS/E](https://img.shields.io/badge/PSS%2FE-1F3864?style=flat) ![AutoCAD](https://img.shields.io/badge/AutoCAD-1F3864?style=flat) ![EPLAN](https://img.shields.io/badge/EPLAN-1F3864?style=flat) ![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=flat&logo=kicad&logoColor=white) ![Altium](https://img.shields.io/badge/Altium-1F3864?style=flat)

**⚡ Power systems and utilities:** HV/MV/ELV planning and design, SLDs, substation design (11 kV / 132 kV / 500 kV), protection and control, selectivity, power system calculations and studies, load flow, load forecasting, feeder planning, generation interconnection and system expansion, transfer analysis, grounding, cable and conduit planning, arc flash evaluation (IEEE 1584, NFPA), switchgear, interlocking logic, commissioning protocols, initial energization, operation and maintenance, BOM/BOQ, technical specifications, reading datasheets, client standards, NESC, wiring regulations.

**🧰 Power and design software:** ETAP, PSS/E, EasyPower, SKM, MATLAB/Simulink, AutoCAD, EPLAN, COMOS, Bentley Station, KiCad, Altium, DipTrace, Proteus, SPICE tools, MS Office.

**🔌 Embedded systems:** PIC32 (MIPS32 M4K), PIC, STM32, ARM Cortex M, NXP Kinetis/LPC, ESP32, WIZnet W5500, bare metal firmware, register level development, HAL and driver layers, FreeRTOS, bootloaders, secure OTA, firmware upgrades and extraction, MISRA-C, static analysis, low power design, edge AI, MPLAB, STM32Cube, JTAG, logic analyzer, power analyzer.

**📡 Communication and protocols:** DLMS/COSEM, Modbus RTU, RS485, RS232, UART, I2C, SPI, CAN, USB, Ethernet, TCP/IP, WebSocket, MQTT, BLE, Wi-Fi, LTE, mesh networks, CC1101, OpenADR 2.0b, SSL.

**🧪 Hardware and electronics:** PCB and board design, signal integrity, EMI/EMC, power supplies, buck/boost converters, PFC, motor control (FOC, BLDC), BMS and SoC/SoH, opto isolators, MOSFETs, ADC, RTC, vibration and acoustic sensing, ORP and pH monitoring, custom dev boards, hardware design, reverse engineering, LCSC and JLCPCB workflow.

**🏭 Industrial and field:** SCADA, DCS, PLC, HMI, field signal testing, site installation and inspection, surveys, QA/QC, stress level testing, fire alarm, CCTV, HSE, supervision.

**📈 Software, data and open source:** Python, R, pandas, Plotly, XGBoost, GBLinear, time series load forecasting, model explainability, unit testing, regression and mutation testing, pytest and unittest, flake8, CI/CD, Git and GitHub, fork and pull request workflow, DCO sign off, Conventional Commits, jupytext, uv, Google Colab, qEEG Pro, PsychoPy.

**🧠 Professional skills:** technical documentation, user manuals, test plans and procedures, project reporting and status reporting, project management and coordination, proposals and quotations, technical leadership, design reviews, decision making, team based problem solving, knowledge sharing.

**📜 Standards:** IEC/EN/UL/IEEE, NFPA, NESC, IEEE 1584, ABET/PEC/PE/FE.

---

# 🏅 Leadership and Activities

- **Campus Director**, Hult Prize (2025)
- **Tech Lead**, Youth Robotec (2023, 2024)
- **Management Head**, IEEE Student Chapter, UET Peshawar (2022): organized seminars and events
- **NaviCart** (startup): electrical project engineer and media team; won the campus rounds of the Zindigi prize
- **Rduinotronics** (startup): project development and PCB STEM instructor
- **ZypherEV** (startup): media team

**🗣️ Languages:** English (fluent), Urdu (fluent)

---

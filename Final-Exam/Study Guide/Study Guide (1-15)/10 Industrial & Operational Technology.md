Industrial and operational technology (OT) systems control physical processes such as pumps, motors, sensors, or assembly lines.  
Unlike IT systems, OT prioritizes availability and safety over confidentiality.  
Your exam will focus on distinguishing different OT system types, understanding supervisory vs. direct control, recognizing automation components, and identifying security risks created by IT/OT convergence.

---

## 10.1 Types of Industrial Control Systems (ICS)

| System Type | Expanded Definition | Nested Key Points (Comparisons) | Workplace Example |
|-------------|----------------------|----------------------------------|--------------------|
| ★ ICS (Industrial Control Systems) | Umbrella term for systems managing industrial and physical processes. | • Includes SCADA, DCS, PLC<br>• Real-time operations<br>• Safety-critical | Used by industries managing HVAC, energy, utilities (not typically EisnerAmper-specific but relevant for clients). |
| SCADA (Supervisory Control and Data Acquisition) | Centralized system that monitors and controls geographically distributed assets. | • Supervisory, not always direct control<br>• Often communicates over long distances | Monitoring pipeline pressures or utility grids for a client’s industrial portfolio. |
| DCS (Distributed Control System) | Localized system controlling processes within a single industrial facility. | • Highly reliable<br>• Direct control of equipment<br>• Multiple controllers across site | Managing automation inside a manufacturing plant or refinery owned by a client. |
| PLC (Programmable Logic Controller) | Ruggedized computer that directly controls physical devices. | • Executes automation logic<br>• Hardware-level control<br>• Fast, deterministic responses | A PLC controlling pumps or valves at a wastewater facility acquired by a client fund. |
| RTU (Remote Terminal Unit) | Field device used in SCADA for remote data collection and control. | • Communicates sensor readings<br>• Executes limited remote actions | Remote sensors providing operational data for infrastructure clients. |
| Comparison | SCADA = supervisory; DCS = localized facility-wide control; PLC/RTU = direct device control. | • PLC = closest to physical hardware<br>• SCADA = broad monitoring<br>• DCS = full plant control | EisnerAmper clients in energy/industrial portfolios rely on these models. |

---

## 10.2 Direct Control vs Supervisory Control

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|---------|----------------------|--------------------|--------------------|
| Direct Control | OT system directly actuates equipment (motors, pumps, valves). | • PLC-level logic<br>• Immediate system response | PLC opening/closing valves in water utility operations. |
| Supervisory Control | High-level guidance and monitoring; does not actuate devices directly. | • SCADA-level<br>• Sends commands to PLCs/RTUs | A SCADA dashboard showing tank levels and sending instructions to PLCs. |
| Comparison | Direct = immediate physical changes; Supervisory = monitoring + high-level commands. | • Exam will test which systems do what | Distinguishing SCADA (supervisory) from PLC (direct). |

---

## 10.3 OT Automation Components

| Component | Expanded Definition | Nested Key Points | Workplace Example |
|-----------|----------------------|--------------------|--------------------|
| Sensors | Devices measuring physical conditions. | • Temperature<br>• Pressure<br>• Flow | Tracking operational metrics at industrial facilities owned by a client fund. |
| Actuators | Convert commands into physical movement. | • Motors<br>• Switches<br>• Valves | Actuator opens/close valves in HVAC system. |
| Human-Machine Interface (HMI) | Interface operators use to monitor and control systems. | • Graphical dashboard<br>• Displays alarms | SCADA HMI used by plant operators at a manufacturing site. |
| Control Logic | Automated rules executed by PLC or DCS. | • Determines how equipment responds<br>• Safety features | Automation logic preventing pump overload. |

---

## 10.4 IT/OT Convergence & Security Implications

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|---------|----------------------|--------------------|--------------------|
| ★ IT/OT Convergence | Connecting OT systems to IT networks for efficiency, monitoring, and analytics. | • Increases attack surface<br>• Requires segmentation<br>• Bridging legacy systems with modern networks | EisnerAmper clients using cloud dashboards to monitor industrial assets. |
| Unique OT Risks | OT values availability & safety above confidentiality. | • Cannot patch frequently<br>• Legacy systems<br>• Must avoid downtime | Delays in patching PLCs or SCADA devices due to operational schedules. |
| Network Segmentation | Separates OT networks from IT networks. | • Prevents malware crossover<br>• Limits blast radius | A ransomware attack on IT systems shouldn't reach industrial controllers. |
| Remote Access Risk | OT systems becoming reachable via the internet or VPN. | • High risk if misconfigured<br>• Requires strict authentication | Attackers exploiting remote access to industrial HVAC or facility systems. |

---

## 10.5 Study Focus Summary

| Exam Topic                    | Explanation                                                 |
| ----------------------------- | ----------------------------------------------------------- |
| Direct vs Supervisory Control | PLC = direct device control; SCADA = supervisory.           |
| ICS Types                     | Know differences between SCADA, DCS, PLC, RTU.              |
| OT Priorities                 | Availability and safety over confidentiality.               |
| Convergence Risk              | IT/OT connectivity increases exposure to cyberattacks.      |
| OT Security Strategies        | Segmentation, limited remote access, strict authentication. |
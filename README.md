# CICS-Legacy-to-Modern-CRUD

Modernizing a COBOL CRUD Application: Mainframe Screens to Modern Architecture.

<p align="center">
  <img src="images/Screen.png" alt="CICS Modernization Dashboard" width="700"/>
  <br>
  <em>CICS Mainframe Modernization Project (Sept 2026)</em>
</p>

## Overview

This repository documents the modernization path for a legacy COBOL CRUD (Create, Read, Update, Delete) application running under CICS (Customer Information Control System) on an IBM z/OS mainframe. The project transitions a fixed-field terminal application into a flexible, service-oriented architecture.

---

## Technical Components & File Directory

This project combines traditional mainframe assets with modern DevOps tooling. The source code is organized as follows:
## 📸 Project Resources

Below is a snapshot of the resources created during the CICS Legacy-to-Modern project, including the COBOL program, BMS map, JCL, VSAM definitions, CICS commands, troubleshooting documentation, and development tools.

![CICS Legacy-to-Modern Project Resources](images/IMG_5113.jpeg)

### [<img src="https://raw.githubusercontent.com/microsoft/vscode/main/resources/linux/code.png" width="20" alt="VS Code icon" /> VS Code / TSO/ISPF Tools](#vscode-tools)

This section includes links and cross-references for developing with IBM Z Open Editor:

| Asset | Description |
| :--- | :--- |
| **Code Links PDF** | Documentation linking modern editor features to TSO/ISPF counterparts. |
| **MAP: JCL** | JCL source for BMS Mapset compilation. |
| **Copybook Source** | Shared COBOL definitions (Linkage Section). |

---

### [<img src="https://img.icons8.com/wired/64/000000/mainframe.png" width="20" alt="Mainframe icon" /> TSO/ISPF & VSAM Data](#mainframe-source)

Source and definitions for the mainframe components:

- `mainframe/jcl/VSAM_DEF.jcl`: VSAM KSDS cluster definition.<img src="images/IMG_5107.jpeg" alt="vsam" width="700"/>
- `mainframe/cobol/CICS_CRUD.cbl`: Main COBOL CICS program source.<img src="images/IMG_5114.jpeg" alt="CICS cobol" width="700"/>
- `mainframe/bms/CICS_MAP.bms`: Basic Mapping Support mapset source.<img src="images/IMG_5109.jpeg" alt="CICS cobol" width="700"/>

### VSAM Operations & Workflows

Documented application flow and command usage for database operations:

| Operation | Command Example | Documentation |
| :---: | :--- | :--- |
| **ADD** | `EXEC CICS WRITE` | [Detailed Workflow](images/VSAM_ADD.png) |
| **DELETE** | `EXEC CICS DELETE` | [Detailed Workflow](images/VSAM_DELETE.png) |
| **UPDATE** | `EXEC CICS REWRITE` | [Detailed Workflow](images/VSAM_UPDATE.png) |
| **BROWSE** | `EXEC CICS STARTBR`/`READNEXT` | [Detailed Workflow](images/VSAM_BROWSE.png) |

---

## [<img src="https://img.icons8.com/wired/64/000000/command-line.png" width="20" alt="Command Line icon" /> Mainframe Commands Used](#commands)

The following CICS commands are utilized for testing, debugging, and system management. Click the links for application-specific usage guides:

### [CICS Troubleshooting Guide (PDF)](./Troubleshooting.pdf)
<p align="center">
  <img src="images/IMG_5106.jpeg" alt="CICS Modernization Dashboard" width="700"/>
  <br>
  <em>CICS Mainframe Modernization Project (Sept 2026)</em>
</p>
Quick-reference document covering:

* `CEDA DEFINE` and `INSTALL` commands for mapsets and libraries [[PDF](./Troubleshooting.pdf)][cite: 1]
* `CEMT SET PROGRAM NEWCOPY` execution and status checks [[PDF](./Troubleshooting.pdf)][cite: 1]
* Resolving `LOAD FAILED` errors and setting up custom `DSNAME` allocations [[PDF](./Troubleshooting.pdf)][cite: 1]

---

## Modernized Components

We have integrated the following modernized components:

*   **Container-Based Services** for elastic scaling.
*   **Web Interface (HTML/CSS/JS)** providing a responsive front-end.
*   **REST APIs (Python Flask)** for secure, flexible service calls.
*   **PostgreSQL DB** for high-performance open-source data management.

## Migration Steps

The application transition followed these logic steps:

1.  **Map Field Definition:** Apply unprotected status to key screen fields.
2.  **Data Retrieval:** 'Enter Year' function returns all other record fields.

## Project Transition

### 📸 Project Transition

**BEFORE: Original Screen Capture**  
[![Original Screen Capture](path/to/before-image.png)](https://www.linkedin.com/feed/update/urn:li:ugcPost:7502364357662658560)

Check out the update on [LinkedIn](https://www.linkedin.com/feed/update/urn:li:ugcPost:7502364357662658560).

**AFTER: Modernized Screen Capture**  
![Modernized Screen Capture](path/to/after-image.png)

## Project Status

This modernization effort is currently:

<p align="center">
  **Wrapping Up Soon**
  <br>
  <img src="images/project_status_bar.png" alt="Project status: wrapping up" width="300" />
</p>
<table border="0" width="100%">
<tr>
<td width="50%" valign="top">

### 🛠️ VS Code / TSO/ISPF Tools
* [Code Links PDF](./docs/code-links.pdf)
* [MAP: JCL](./jcl/map.jcl)
* [Copybook Source](./cobol/copybooks/)

---

### 💾 TSO/ISPF & VSAM Data
* **VSAM:** JCL
* **Program Source**
* **BMS Mapset Source**
* **VSAM Operations:** `ADD`, `DELETE`, `BROWSE`, `UPDATE`

---

### 💻 Mainframe Commands Used
* `CEMT`, `CEDF`: Brief command usage
* `CEDF`: Operation used commands usage
* `CEMT`: Add three field command usage
* `BROWSE`: Add/Delete usage
* `UPDATE`: Update/Find command usage

---

### 🎥 CICS Demo (Sept 2026)
[![CICS Demo](https://img.youtube.com/vi/YOUR_VIDEO_ID/maxresdefault.jpg)](https://www.youtube.com/watch?v=YOUR_VIDEO_ID)

</td>
<td width="50%" valign="top">

### 🚀 Modernized Components
**Modernized components added:**
* Container-Based Services
* Web Interface (HTML/CSS/JS)
* REST APIs (Python Flask)
* PostgreSQL DB

---

### 📋 Migration Steps
`1. Apply unprotected to key fields` ➔ `2. Enter Year: Returns other fields`

---

### 📸 Project Transition

### 📸 Project Transition

**BEFORE: Original Screen Capture**  
![BEFORE](./assets/before-screen.png)

Here is my latest project update:

[![View LinkedIn Post](https://img.shields.io/badge/LinkedIn-View_Project_Update-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/feed/update/urn:li:ugcPost:7502364357662658560)

Check out the repository below for details.  

**AFTER: Modernized Screen Capture**  
![AFTER](./assets/after-screen.png)

---

### 📊 Example of issues I experienced
** VSAM Record Update Issue**
 
Problem: When I updated a record, fields like Role/Title and Skills were getting blanked out.
Cause: The program was moving the screen data before the VSAM READ UPDATE, which replaced my changes with the old record.
Fix: I changed the order so the screen data is moved after the READ UPDATE and before the REWRITE. This allowed my updated information to save correctly.
![AFTER](./assets/after-screen.png)
**VSAM Record Layout Issue**
 
Problem: Some data was shifting, getting truncated, or not saving correctly.
Cause: The Working-Storage record layout didn't fully match the VSAM record structure.
Fix: I aligned the record layout to the VSAM file at 205 bytes, making sure the fields matched correctly when moving data between the screen and VSAM
![AFTER](./assets/after-screen.png)
</td>
</tr>
</table>
---


[Github Repository Mockup Visualization Reference](images/README_Storyboard.png)

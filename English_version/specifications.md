# Project Brief: Disaster Networking

**February – April 2025**  
Maxime Bossant, Antonia Ivanova, Maxence Maury, Erwan Poncin  

---

## Table of Contents  
1. [Project Overview](#project-overview)  
2. [Project Target](#project-target)  
3. [Our Budget](#our-budget)  
4. [Timeline](#timeline)  
5. [Functional Specifications](#functional-specifications)  
6. [Technical Specifications](#technical-specifications)  

---

## Project Overview  

The title of our project is **Disaster Networking**.  
We studied the use of **LoRa** technology to set up a resilient communication network that can operate in the event of a natural disaster, when traditional infrastructures are down.  

The selected case study is **Cyclone Chido**, which hit Mayotte in December 2024 and took down **51 out of 54** mobile network antennas. The objective is to **prepare** a network resistant to this type of event, to allow **rescue workers** and **residents** to continue exchanging vital information.  

---

## Project Target  

The project is based on a preventive approach: **anticipating the disaster** by deploying a network adapted to the area's topography and density.  

We tested two LoRa frequency bands (433 MHz and 868 MHz) in urban, peri-urban, and rural environments.  
We used the **Meshtastic** protocol, a self-routing mesh network protocol, deployed on different boards.  

The project deliverables are:  
- A **decision tree** to help choose frequency and network topology based on terrain.  
- **Range test results** for LoRa under various factors (height, urban density, temperature, distance).  
- A **deployment guide** for Meshtastic equipment.  

---

## Our Budget  

We had a budget of **54 hours of work per person** in a group of 4, that is **216 hours** or **27 person-days**.  

---

## Timeline  

- **Project start**: February 2025  
- **Mid-term presentation**: March 10, 2025  
- **Final presentation**: April 7, 2025  

---

## Functional Specifications  

### Functional Objectives Achieved  
- Test and compare the performance of **LoRa 433 MHz** and **LoRa 868 MHz**.  
- Evaluate the impact of **antenna height**, **urban density**, **temperature**, and **distance**.  
- Determine the **optimal configurations** depending on the environment.  
- Propose a **field-oriented deployment guide**, with practical recommendations.  

### Key Deliverable  
- A **decision tree** (Appendix 1) indicating hardware, frequency, topology, and height to use based on terrain configuration.  

---

## Technical Specifications  

### Infrastructure and Hardware  

- **Technology used**: LoRa (Long Range), Meshtastic (open-source firmware)  
- **Frequencies tested**: 433 MHz, 868 MHz  

#### Hardware used:
- **433 MHz**:  
  - 4x T-BEAM Supreme (LilyGO)  

- **868 MHz**:  
  - 2x T-BEAM Supreme (LilyGO)  
  - 1x WiFi LoRa 32 (Heltec)  
  - 1x Wio-WM1110 (Seeed Studio)  

### Networking and Protocol  
- **Meshtastic**:  
  - Automated mesh network with dynamic routing.  
  - Point-to-point communication via LoRa.  
  - Bluetooth/Wi-Fi compatibility for smartphone interface.  

- **Porting Meshtastic to other boards** was partially attempted (via manual flashing) but was abandoned in favor of field testing, which was deemed a priority.  

### Performance and Range (actual results)  
- **Observed range**:  
  - **433 MHz**:  
    - Dense urban: up to 500 m  
    - Open rural: up to 1.5 km  
  - **868 MHz**:  
    - Urban: up to 1.5 km  
    - Open rural: up to 5 km  

- **Optimal height**:  
  - Urban: antenna at ~10 m (equivalent to 3rd floor)  
  - Rural: ~5 m is sufficient  

### Power Consumption and Autonomy  
- **Theoretical estimate**: >48 h of autonomy in low power mode  
- **No exact measurements** were taken regarding autonomy  

### Robustness  
- Tests limited to outdoor environments under normal conditions  
- Sensitivity to external power and casing was not studied  

### Deployment and Maintenance  
- **Meshtastic flashing documentation** for T-BEAM and other boards (see Appendix 3)  
- **Simplified deployment guide** based on terrain  
- No supervision or monitoring system was integrated into the project  


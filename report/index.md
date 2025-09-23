# Smart Home Dashboard — Project Report

## 🌟 Introduction
The vision was simple: controlling a smart home should feel as natural as tapping on a floor plan.  

To bring this idea to life, our team built a **custom smart home dashboard** using **Home Assistant** as the backbone, **Aqara devices** for control, and the **Matter protocol** for seamless connectivity.  

---

## 🏡 Features Implemented
- **Floor Plan Dashboard** – visual layout of the home for device interaction  
- **Room-Level Switching** – single-tap on/off for devices or entire rooms  
- **Curtain Controller** – percentage-based open/close flexibility  
- **Automated Scenes** – *Goodnight* to switch off everything, *Good Morning* to light up the lobby  

---

## ⚙️ Technology Stack
- **Home Assistant** (open-source home automation platform)  
- **Matter Protocol** (interoperability across devices)  
- **Aqara Switches** and sensors for device integration  
- **YAML Configuration** for dashboard customization  

---

## 📂 Proof of Implementation
YAML configuration files are available in the [`yaml-proof`](../yaml-proof) folder.  

Example snippet:

```yaml
type: picture-elements
image: /local/images/floorplan.png
elements:
  - type: state-icon
    entity: light.living_room
    style:
      top: 40%
      left: 30%

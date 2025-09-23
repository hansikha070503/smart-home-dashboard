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
YAML configuration files are available in the [`yaml-proof`](yaml-proof/floor_plan.yaml) folder.  

Example snippet:

```yaml
views:
  - title: Home
    sections:
      - type: grid
        cards:
          - type: picture-elements
            elements:
              - type: image
                entity: light.aqara_smart_wall_switch_z1_pro_3
                image: mr3fan
                state_image:
                  'on': /local/icons/fan_offf.png
                  'off': /local/icons/fan_off.png
                tap_action:
                  action: toggle
.
.
```
---

## 📸 Dashboard
![Dashboard Preview](images/dashboard.png)


---


## 🎥 Videos


<div align="center">


| Room-Level Switching | Curtain Automation | Goodnight & Good Morning Scenes |
|:--------------------:|:------------------:|:-----------------------------:|
| <video width="250" controls><source src="videos/room_video.mp4" type="video/mp4"></video><br>[▶️ Watch / Download](videos/room_video.mp4) | <video width="250" controls><source src="videos/curtain_video.mp4" type="video/mp4"></video><br>[▶️ Watch / Download](videos/curtain_video.mp4) | <video width="250" controls><source src="videos/gn_gm_video.mp4" type="video/mp4"></video><br>[▶️ Watch / Download](videos/gn_gm_video.mp4) |

</div>

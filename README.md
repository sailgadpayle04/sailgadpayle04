<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=28&duration=2500&pause=500&color=0e6e55&center=true&width=700&lines=Hi+👋+I'm+Sail+Gadpayle;Firmware+%26+Embedded+Engineer+⚙️;ARM+Cortex-M+%7C+Bare-Metal+C;Low-Power+%7C+BLE+%7C+VLSI;Building+Close+to+the+Metal+🔩" alt="Typing SVG" />
</div>

<br/>

---

## 🌟 About Me

I'm an **Electronics & Firmware Engineer** currently interning at **Rurutek Pvt Ltd**, Chengalpattu, India — working on embedded firmware and hardware bring-up. I specialize in **bare-metal C**, **low-power system design**, and **register-level peripheral drivers** on ARM Cortex-M platforms.

Finishing my **B.Tech in Electronics Engineering** (Honors: VLSI Design) at YCCE Nagpur — graduating 2026.

**🎯 Current Focus:**
- 🔋 Low-power firmware — sleep modes, RTC wakeup, power budgeting
- ⚙️ Bare-metal bootloaders, linker scripts, and memory management
- 📡 BLE firmware — GATT services, nRF Connect SDK (Zephyr RTOS)
- 🧠 VLSI design fundamentals and SystemVerilog verification

---

## 🛠️ Tech Stack

### 💻 Languages
<div align="left">

![C](https://img.shields.io/badge/Embedded_C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Verilog](https://img.shields.io/badge/Verilog%20%2F%20SystemVerilog-E81828?style=for-the-badge&logoColor=white)

</div>

### ⚙️ Hardware & Embedded
<div align="left">

![STM32](https://img.shields.io/badge/STM32-03234B?style=for-the-badge&logo=stmicroelectronics&logoColor=white)
![ARM](https://img.shields.io/badge/ARM_Cortex--M-0091BD?style=for-the-badge&logo=arm&logoColor=white)
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white)
![BLE](https://img.shields.io/badge/BLE_GATT%2FGAP-0082FC?style=for-the-badge&logo=bluetooth&logoColor=white)
![VLSI](https://img.shields.io/badge/VLSI_Design-FFD60A?style=for-the-badge&logoColor=black)

</div>

### 🔌 Protocols
<div align="left">

![UART](https://img.shields.io/badge/UART-FF6B6B?style=for-the-badge&logoColor=white)
![SPI](https://img.shields.io/badge/SPI-4ECDC4?style=for-the-badge&logoColor=white)
![I2C](https://img.shields.io/badge/I2C-45B7D1?style=for-the-badge&logoColor=white)
![MQTT](https://img.shields.io/badge/HTTP%20%2F%20MQTT-660066?style=for-the-badge&logo=mqtt&logoColor=white)

</div>

### 🛠️ Tools & IDEs
<div align="left">

![STM32CubeIDE](https://img.shields.io/badge/STM32CubeIDE-03234B?style=for-the-badge&logo=stmicroelectronics&logoColor=white)
![Keil](https://img.shields.io/badge/Keil_μVision-0066CC?style=for-the-badge&logoColor=white)
![VSCode](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![EasyEDA](https://img.shields.io/badge/EasyEDA-1565C0?style=for-the-badge&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

</div>

### 🐧 Operating Systems
<div align="left">

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Debian](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)
![Arch](https://img.shields.io/badge/Arch_Linux-1793D1?style=for-the-badge&logo=archlinux&logoColor=white)
![Fedora](https://img.shields.io/badge/Fedora-294172?style=for-the-badge&logo=fedora&logoColor=white)

</div>

---

## 🚀 Featured Projects

### 🔋 Low-Power Data Logger with Flash Storage
<img src="https://img.shields.io/badge/Status-✨_Complete-0e6e55?style=flat-square" alt="Status"/>
<img src="https://img.shields.io/badge/Platform-STM32_ARM_Cortex--M-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white" alt="Platform"/>
<img src="https://img.shields.io/badge/Difficulty-Intermediate-FFD60A?style=flat-square" alt="Difficulty"/>

**A battery-operated sensor data logger designed around ultra-low power operation**

**🎯 Key Features:**
- 🔋 **< 10 µA idle** — MCU enters STOP mode after each write, woken by RTC alarm
- 💾 **W25Q32 SPI Flash** with **LittleFS** file system — wear-levelling and atomic writes for data safety across power-loss events
- 🔌 **Register-level SPI driver** — page-program, sector-erase, status-register polling; byte-level timing validated on DSO
- 📊 **Full power budget documented** — current profiled across Run, Sleep, and STOP modes using a shunt resistor

**🏷️ Stack:**
`STM32` `ARM Cortex-M` `Embedded C` `SPI` `LittleFS` `RTC` `Low-Power` `DSO`

---

### ⚙️ UART Bootloader for Firmware Update
<img src="https://img.shields.io/badge/Status-✨_Complete-0e6e55?style=flat-square" alt="Status"/>
<img src="https://img.shields.io/badge/Platform-STM32F1_Bare--Metal-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white" alt="Platform"/>
<img src="https://img.shields.io/badge/Difficulty-Advanced-FF4136?style=flat-square" alt="Difficulty"/>

**A custom Stage-1 bootloader for in-field firmware updates over UART — no external programmer needed**

**🎯 Key Features:**
- 📥 **XMODEM receive** — opens a UART listen window at reset; accepts new binary, programs the application flash sector
- ✅ **CRC-32 verification** — retains old firmware intact on checksum mismatch, preventing a brick on a bad transfer
- 🗺️ **Custom linker script** — bootloader at `0x08000000`, application at `0x08004000`; startup remaps VTOR and sets MSP for clean hand-off
- 🐍 **Python host script** — automates the flashing workflow from PC over any serial port

**🏷️ Stack:**
`STM32F1` `Bare-Metal C` `UART` `XMODEM` `CRC-32` `Linker Script` `VTOR` `Python`

---

## 📫 Connect With Me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sailgadpayle)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sailgadpayle04@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sailgadpayle)

</div>

---

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=sailgadpayle&color=0e6e55&style=flat-square&label=Profile+Views" alt="Profile views" />
</div>

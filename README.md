# Bar-Type & Custom TFT LCD Engineering Knowledge Base

Welcome to the open technical repository of **Sunshine Display**. This repository serves as a professional engineering reference for hardware designers, embedded systems engineers, and B2B procurement specialists looking for reliable bar-type and custom TFT LCD module solutions.

---

## 📌 Table of Contents
1. [Bar-Type TFT LCD Selection Guide](#1-bar-type-tft-lcd-selection-guide)
2. [Common FPC (Flexible Printed Circuit) Definitions](#2-common-fpc-flexible-printed-circuit-definitions)
3. [LCD Interface Comparison (SPI vs. RGB vs. MIPI vs. MCU)](#3-lcd-interface-comparison)
4. [Provided Sample Datasheets](#4-provided-sample-datasheets)
5. [Contact & Custom Solutions](#5-contact--custom-solutions)

---

## 1. Bar-Type TFT LCD Selection Guide
Bar-type (cut-type or custom-aspect-ratio) TFT LCDs are widely used in industrial equipment, smart home appliances, automotive dashboards, and shelf edge displays. Key factors to evaluate during selection include:
* **Active Area & Aspect Ratio:** Ensuring the mechanical cutout matches your enclosure constraints.
* **Brightness (Nits):** Standard indoor modules range from 250–400 nits, whereas sunlight-readable outdoor displays require **800 to 1500+ nits** with IPS wide-view angles.
* **Operating Temperature:** Industrial-grade panels typically withstand `-20°C to +70°C` (or wider ranges for automotive use).

---

## 2. Common FPC (Flexible Printed Circuit) Definitions
The FPC interface is critical for signal transmission and mechanical stability. A standard industrial TFT module FPC typically groups pins into:
* **Power Supply:** VCC, LED+ / LED- (Backlight anode and cathode).
* **Control & Data Signals:** CS, Reset, D/C (Data/Command), SCL/SDA (for SPI).
* **Interface Bus Lines:** Depending on the protocol, dedicated lanes for RGB parallel data or high-speed MIPI differential pairs.
* **Touch Panel Integration:** I2C interface lines (SDA/SCL, INT, RST) if a capacitive touch panel (CTP) is bonded.

---

## 3. LCD Interface Comparison
Choosing the right interface depends on your host processor (MCU, MPU, or SoC) performance and pin availability:

| Interface Type | Typical Resolution | Speed / Bandwidth | Pin Count | Best Application |
| :--- | :--- | :--- | :--- | :--- |
| **SPI (3-wire / 4-wire)** | Low to Medium (e.g., QVGA) | Moderate | Low (3-5 pins) | Simple UI, cost-sensitive devices, small wearables. |
| **MCU 8080 / 6800** | Medium (e.g., WVGA) | Fast (Parallel bus) | High (8/16 data pins) | Embedded MCUs with internal graphics controllers. |
| **RGB Parallel** | Medium to High (up to 720p) | High | High (16-24 pins) | MPUs / Linux processors requiring direct frame buffer. |
| **MIPI DSI** | High to Ultra-High (HD/FHD) | Very High (Differential) | Very Low (2-4 lanes) | Modern smartphones, high-end automotive, medical tablets. |

---

## 4. Provided Sample Datasheets
* **[SDT0286BHSI-01.pdf](./SDT0286BHSI-01.pdf)**: Detailed specification sheet for our standard bar-type TFT LCD module sample.

---

## 5. Contact & Custom Solutions
Need custom FPC shape, customized pinouts, high-brightness enhancement, or optical bonding (OCA/OCR)? 

* **Official Website:** [Sunshine Display](https://www.sunshinelcd.com)[cite: 1]
* **Inquiry & Support:** Visit our website to download full CAD drawings and request engineering sample validation.

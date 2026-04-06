# AlgaeTower
AlgaeTower 是一台垂直長筒形閉環微藻系統，專為離網與極端環境設計。可自動培養微藻、收穫濃縮、乳酸發酵，並產出可塑型營養泥，同時回收 CO₂ 與水分。 系統採用三隔間培養（50% 產油、25% 高蛋白、25% 高澱粉），以太陽能為主能源，Stirling 引擎輔助回收油脂發電。第三層乳酸發酵提升口感與吸收率，最終擠出可食用營養泥。 室內無光時每日耗電約 5.5–6.8 kWh，有陽光輔助時自給率大幅提升。每月僅需補充微量元素與純水。 AlgaeTower 強調簡單可靠、模組化維護，適合離網生活，也可作為太空生命支持原型。
# AlgaeTower v1.1 Final

**Open Source Closed-Loop Microalgae Nutrition Paste Machine**  
**開放源碼閉環微藻營養泥製造機（極端環境適用版）**

## Overview / 專案簡介

AlgaeTower is a vertical cylindrical, fully automatic, closed-loop microalgae system designed for off-grid homes and extreme enclosed environments (space stations, Mars bases).  
It produces edible lactic acid fermented nutrition paste while recycling CO₂, water, and partial waste.

本專案是一台垂直長筒形全自動閉環微藻系統，適合離網家庭與極端封閉環境使用，可產出可食用的乳酸發酵營養泥，同時回收 CO₂、水分與部分廢物。

誠實面對熱力學現實：完全自給電非常困難，因此以自然陽光 + 太陽能板為主要能源，Stirling 引擎作為廢熱與廢藻泥回收輔助裝置。這是經過多次優化後，最務實、可複製的版本。

## Key Features / 主要特點

- Modular 4-layer design / 模組化 4 層設計，可獨立拆裝維護
- UV-C sterilization feeding boxes / UV 殺菌投料小箱（第1層與第3層）
- Adjustable compartments in Layer 1 (50% high-lipid, 25% high-protein, 25% high-starch) / 第一層可調整隔間培養（50% 產油藻、25% 高蛋白、25% 高澱粉）
- Dedicated oil extraction channel in Layer 2 (65–75% oil for power generation) / 第二層專用榨油通道（65–75% 油脂用於發電）
- Lactic acid fermentation in Layer 3 for better taste and digestibility / 第三層乳酸發酵，提升口感與吸收率
- Mode switching (food priority / power assist) / 模式切換（食物優先 / 發電輔助）
- Hybrid energy: solar primary + Stirling auxiliary / 太陽能為主 + Stirling 輔助回收

## Specifications / 規格

- Diameter: 130–140 cm / 直徑：130–140 cm
- Height: 180–200 cm / 總高：180–200 cm
- Culture volume (Layer 1): 650–800 L / 培養液量（第1層）：650–800 L
- Daily output: 800–1000 g wet fermented nutrition paste (25–35% solids) / 日產量：800–1000 g 濕發酵營養泥（固形物 25–35%）
- Total weight: \~1.1–1.3 tons / 總重量：約 1.1–1.3 噸

## Energy Reality / 能源現實說明

In indoor conditions without natural light, daily power consumption is approximately 5.5–6.8 kWh.  
Stirling recovery provides about 0.45–0.65 kWh.  
It is recommended to use solar panels to significantly reduce external charging needs.

在室內無自然光的情況下，每日耗電約 5.5–6.8 kWh。Stirling 回收電量約 0.45–0.65 kWh。建議搭配太陽能板使用，以大幅降低外部充電需求。

有自然陽光或太陽能輔助時，LED 耗電可下降 40–60%，總耗電降至 2.5–4.0 kWh/天，自給率明顯提升。

## 4-Layer Structure / 4層結構

**Layer 1: Cultivation Growth Chamber / 第1層：培養生長室**  
Divided into 3 compartments with adjustable ratios (50% high-lipid, 25% high-protein, 25% high-starch).  
Lighting: One vertical long LED tube per compartment + high-reflectivity mirror walls (20–50 Hz PWM + dynamic duty cycle).  
Venturi microbubble generator (tangential injection) + air-lift circulation.  
UV-C sterilization feeding box at top.  
Air inlet with HEPA filter.  
Inner walls with food-grade anti-fouling coating.

**Layer 2: Harvesting & Mild Concentration Chamber / 第2層：收穫與溫和濃縮室**  
Central UV lamp (35–38°C).  
Conical spiral screw + 0.1 mm wedge wire mesh.  
Automatic backwash nozzles + low-power ultrasound.  
Dedicated oil extraction channel for lipid compartment (65–75% oil for power generation).  
Water ring pump for water return and vacuum concentration.  
Target solids: 25–32%.

**Layer 3: Lactic Acid Fermentation & Shaping Chamber / 第3層：乳酸發酵與塑型室**  
Low-speed stirrer + temperature control (30–35°C).  
pH sensor + short anaerobic mode.  
Lactiplantibacillus plantarum fermentation (auto-seeding + backup inoculum port).  
UV-C sterilization feeding box.  
Spiral extrusion head with interchangeable molds for moldable fermented nutrition paste.

**Layer 4: Auxiliary Energy Recovery Chamber / 第4層：輔助能源回收室**  
Stirling external combustion engine (auxiliary power from excess biomass/oil).  
Large capacity battery.  
External power interface (mainly for cold start and backup).  
Staged heat recovery + exhaust condenser + UV gas disinfection.

## Base & Structure / 底座與結構
- Three-point support base with counterweight and shock absorption system.  
- Tower body with circumferential reinforcing rings.

## Control System / 控制系統
- Arduino-based controller with essential sensors (pH, temperature, pressure, liquid level).  
- Main functions: scheduled harvesting, backwash, gas relief, dynamic LED adjustment.  
- When Layer 1 starts harvesting, automatically dim Layer 1 LEDs and put Layer 2 & 3 into low-power standby mode.

## License / 授權
CC BY-SA 4.0 (hardware) + GPLv3 (software)

## Contributing / 貢獻
Welcome to fork, improve, and contribute!  
歡迎 Fork、改進與貢獻！

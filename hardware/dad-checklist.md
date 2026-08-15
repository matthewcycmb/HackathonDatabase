# Sun Cheong shopping checklist (for Dad)

**Shop:** Sun Cheong Computer Co. 新昌電腦有限公司 — G/F, **246 Apliu Street**, Sham Shui Po 深水埗鴨寮街246號地下 · 11:00–20:00 daily · WhatsApp +852 9319 5163 · https://scccltd.com
Careful: "Sun Cheong Electricals" at 171 Apliu St is a different shop — go to **246**.

Prices are from the shop's own catalog (scccltd.com, Aug 2026). Derived from 40 verified prize-winning hardware hackathon projects (see winning-projects-analysis.md). Matthew already owns: ESP32 devkit, MAX30102 heart-rate, MPU6050 IMU, M5Stack CoreS3 — this list fills the gaps.

## Tier 1 — buy no matter what (~HK$415)

| Item | 中文 | HKD | Why (evidence) |
|---|---|---|---|
| ESP32-CAM (OV2640) | ESP32-CAM 鏡頭模組 | 78 | Cameras in 8/40 winners; ESP32-CAM named in 3 |
| ESP32-CAM-MB USB programmer | ESP32-CAM 下載底板 | 35 | Needed to flash the CAM easily |
| MAX98357A I2S amp | MAX98357A I2S 功放模組 | 25 | Audio output in 10/40 winners |
| Speaker 3W 4Ω | 小喇叭 3W 4Ω | 18 | Pairs with amp |
| SG90 servo ×2 | SG90 9g 舵機 ×2 | 50 | Servos in 7/40 winners |
| OLED 0.96"-class (SSD1306) | 0.96吋 OLED 顯示屏 | 45 | Small displays in 10/40 winners |
| INMP441 I2S microphone | INMP441 I2S 麥克風模組 | 25 | Mics in 7/40 winners |
| HC-SR04 ultrasonic | HC-SR04 超聲波模組 | 19 | 3/40 winners; robot staple |
| Vibration motor module ×2 | 震動馬達模組 ×2 | 24 | Haptics in 4/40; huge demo feel |
| TP4056 Type-C charger | TP4056 Type-C 充電模組 | 10 | Portable demos |
| LiPo battery 1000–2000mAh | 鋰電池 1000–2000mAh | 20 | Portable demos |
| Type-C charge/discharge board | Type-C 充放電模組 | 10 | Clean 5V from battery |
| Breadboard 400-pt | 麵包板 400孔 | 15 | |
| Jumper wires M-F 40-pin | 杜邦線 公對母 | 20 | |
| Grove-to-DuPont cables ×2 | Grove 轉杜邦線 ×2 | 20 | Wires CoreS3 to everything above |

## Tier 2 — strongly recommended (~HK$285)

| Item | 中文 | HKD | Why |
|---|---|---|---|
| Extra ESP32 DevKit V1 | ESP32 開發板 | 65 | ESP32 in 13/40 winners; spare = demo insurance |
| MG90S metal-gear servo | MG90S 金屬齒輪舵機 | 26 | Stronger joints for robots/wearables |
| TB6612 motor driver | TB6612 電機驅動模組 | 20 | Robot archetype (9/40 winners) |
| TT gear motor + wheel ×2 | TT馬達連車輪 ×2 | 20 | Robot archetype |
| Relay module 1ch | 繼電器模組 1路 | 12 | Smart-object archetype (2/40 named) |
| PIR motion HC-SR501 | 人體紅外感應模組 | 20 | Home-monitoring archetype |
| TFT 1.77" ST7735 | 1.77吋 TFT 顯示屏 | 39 | Richer UI than OLED |
| WS2812B LED strip 1m | WS2812B 燈帶 1米 | 45 | LED displays in 4/40 winners |
| 18650 dual case + DC plug | 18650 電池盒連DC插 | 12 | Robot power |
| 16x2 LCD (I2C) | 1602 液晶屏 (I2C) | ~25, ask | LCDs in 5/40 winners; not in web catalog |

## Tier 3 — if he sees it, grab it

| Item | 中文 | HKD | Why |
|---|---|---|---|
| MLX90614 IR thermometer | MLX90614 紅外測溫模組 | 89 | Contactless temp; health archetype wow-factor |
| GPS module (NEO-6M) | GPS 模組 NEO-6M | ask | 3/40 winners; outdoor archetype |
| LoRa module pair (SX1278) | LoRa 模組 ×2 | ask | Off-grid mesh archetype (minutemesh won with this) |
| Stepper 28BYJ-48 + driver | 步進馬達連驅動板 | ask | Sorting machines (2 winners) |
| MAX9814 analog mic | MAX9814 麥克風模組 | 25 | Backup mic |
| WS2812B LED ring | WS2812B 燈環 | 12–22 | Wearable glow |
| FSR402 force sensor | FSR402 壓力感應器 | 68 | 2/40 winners — only if doing music/health input |

**Skip:** flex sensor (HK$248 in HK retail — badly overpriced; order online later if ever needed).

**Totals:** Tier 1+2 ≈ HK$700. With a couple of Tier 3 picks ≈ HK$850–950. All within HK$500–1,000 target.

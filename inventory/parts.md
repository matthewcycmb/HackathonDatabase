# Parts → Idea Matcher

Owned inventory mapped to buildable project archetypes. Update after every purchase and every retro.

## Owned
| Part | Status | Notes |
|---|---|---|
| ESP32 (38-pin devkit) | ✅ have | WiFi/BT MCU, the workhorse |
| MAX30102 | ✅ have | Heart-rate + SpO2 (health/wearable angle) |
| MPU6050 | ✅ have | 6-axis IMU (motion/gesture/fall detection) |
| M5Stack CoreS3 | 🚚 ordered | ESP32-S3, touchscreen, camera, mic, Grove ports |
| Grove + Grove→DuPont cables | 🚚 ordered | fast wiring, demo-safe vs loose jumpers |

## Buildable archetypes (validated against 40 verified winners — see hardware/winning-projects-analysis.md)
- **Health / assistive wearable (8/40 winners)** — MAX30102 + MPU6050 + ESP32 (+ haptics, OLED, force sensor from haul): stress/fall/rehab monitor. Winners: StabiliKnee (3rd, MakeUofT), ShoulderCupid, Twin (1st, MakeUofT). Emotion hook: aging grandparents, athlete safety.
- **Music / conversational audio object (7/40)** — CoreS3 mic/screen or INMP441 + MAX98357A + speaker + MPU6050 gestures: AI companion object, instrument coach. Winners: TeddyTalk, JamDeck.
- **Vision smart-object (8/40 use cameras)** — CoreS3 built-in camera or ESP32-CAM: wearable vision aid, monitoring object. Winners: Cupid Glasses, Catatouille (grand prize).
- **Robot / actuated machine (9/40)** — needs haul: servos, TB6612, TT motors, HC-SR04. Winners: Litter Critter, Sortify, BARK.
- **Outdoor / off-grid (7/40)** — needs Tier 3: GPS, LoRa. Winners: TrailSense, minutemesh, BreadCrumb Trail.
- **Interactive display (4/40)** — WS2812B strip/ring + MPU6050. Winners: VideoGlobe, AR Cube Cannon.

Buy list to fill the gaps: `hardware/dad-checklist.md`. Parts bought from the haul get moved to Owned.

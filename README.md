# About Me

## 👨‍💻 전진욱 | 임베디드 펌웨어 개발자

> **MCU를 활용한 정밀 제어 펌웨어 개발에 강점을 가진 5년 차 개발자 전진욱입니다.** 전기차 충전기 프로젝트를 통해 `STM32, Atmega`등 다양한 MCU를 다루며 하드웨어의 성능을 최대한으로 이끌어내는 경험을 쌓았습니다.
또한, 펌웨어 개발 역량을 바탕으로 `Linux` 환경에서 `Python`을 이용한 통신 프로토콜 스택을 구현하는 등 임베디드 시스템의 전체적인 흐름을 이해하고 개발하는 능력을 갖추고 있습니다. 안정성과 신뢰성이 최우선인 제어 시스템 설계에 가장 큰 자신감을 가지고 있습니다.

---

### 🛠️ 기술 스택 (Skills)

| 구분 | 능숙 (Proficient) | 경험 (Experienced) |
| :--- | :--- | :--- |
| **MCU & Dev Environment** | `STM32 (G/H series)`, `Atmega`, `Arduino`, `VSCode(PlatformIO)` | `Microchip Studio`, `STM32Cube Series` |
| **RTOS & GUI** | `Tkinter (Python)` | `FreeRTOS`, `TouchGFX` |
| **Communication Protocols**| `UART`, `I2C`, `SPI`, `OCPP 1.6(via Python)` | `ISO15118`, `Websocket`, `MAVLink` |
| **Languages & Tools** | `C`, `Python`, `C++` | `Git`, `Rust`, `JSON`, `SQL` |
| **Hardware & Debugging** | `Oscilloscope`, `Debugger (ST-Link, Atmel ICE)` | - |

---

### 🚀 주요 프로젝트 (Projects)

---

#### 1. 7kW 완속 충전기 펌웨어 및 OCPP 시스템 개발

*   🏢 **소속:** 위지트에너지
*   📅 **기간:** 2024.11 ~ 현재

> **🎯 Project Goal**
>
> KC 인증 및 OCPP 1.6 국제 표준을 만족하는 7kW 완속 충전기를 개발하여 안정성과 신뢰도를 갖춘 상용 제품을 출시하는 것을 목표로 했습니다.



*   **👤 My Role: 펌웨어 개발 리드 및 OCPP HMI 시스템 개발**

    *   **🧗 Challenge 1: 충전 전력과 시퀀스 제어 및 KC 인증 요건 충족**
        *   **Action:** `STM32` 기반의 핵심 펌웨어 로직(충전 시퀀스, 전력/센서 제어)을 주도적으로 설계하고, 시스템 신뢰도 확보를 위해 온도에 따른 충전전력 Throttling 시스템, 자동 복구, 체크섬 검증, OTA 기능을 구현했습니다. KC 인증을 위해 직접 규격을 분석하고 테스트 항목에 대응하는 펌웨어 기능을 개발하여 현장 테스트에 대응했습니다.
        *   **✅ Result:** **KC 61851 - 1 인증을 성공적으로 완료**하여 제품 상용화의 핵심적인 기반을 마련했습니다.

    *   **🧗 Challenge 2: OCPP 1.6 표준 기반의 스마트 충전 기능 구현**
        *   **Action:** `Python`과 `Tkinter`를 기반으로 OCPP 연동 HMI를 협업하여 개발하는 과정에서, `SQL`을 활용하여 로컬 인증 및 충전 스케줄 관리 기능을 구현함으로써 서버 의존도를 낮추고 충전기 단독 동작의 안정성을 높였습니다.
        *   **✅ Result:** SmartCharging 등 핵심 기능을 포함한 **OCPP HMI를 성공적으로 개발**하여 해당 솔루션이 **OCPP 1.6 Full Certification**을 획득하는데 기여하였습니다.

*   **🔧 사용 기술:** `STM32`, `C`, `UART`, `OCPP 1.6 (Python, Tkinter)`, `ISO15118`, `KC61851`, `SQL`

---
#### 2. RTOS 기반 완속충전기 개발(진행중)

*   🏢 **소속:** 위지트에너지
*   📅 **기간:** 2025.07 ~ 현재

> **🎯 Project Goal**
>
> `STM32 H7 Series`를 사용하는 충전기시스템으로, 하나의 칩으로 OCPP 1.6 스택, 충전기 제어, Touch GFX기반 HMI Task를 관리하는 제품을 출시하는 것을 목표로 하고있습니다.  



*   **👤 My Role: TouchGFX 기반 HMI 제작, 충전기 제어시스템, OCPP 1.6 Full Stack(via C++) 개발**

*   **🔧 사용 기술:** `STM32`, `C++`, `UART`, `OCPP1.6(C++)`, `Websocket`, `Touch GFX`

#### 3. Atmega MCU 기반 7kW 충전기 및 OCPP 클라이언트 개발

*   🏢 **소속:** (주)인피니티웍스
*   📅 **기간:** 2021.04 ~ 2024.11

> **🎯 Project Goal**
>
> `Atmega` MCU를 사용하는 7kW 충전기와 한전 서버를 `OCPP 1.6` 프로토콜로 연동하여 원격 제어 및 모니터링 시스템을 구축하는 것을 목표로 했습니다.



*   **👤 My Role: 펌웨어 및 Linux 기반 OCPP 클라이언트 개발**

    *   **🧗 Challenge: 제한된 리소스의 MCU와 외부 통신 시스템 연동**
        *   **Action:** `Atmega` MCU와 Arduino 프레임워크로 주변 장치(LED, 계량기 등) 제어 펌웨어를 개발했습니다. 동시에 `Linux(Ubuntu)` 환경에서 `Python`과 `Websocket`을 이용하여 `OCPP 1.6` 클라이언트를 개발하여 충전기와 서버 간의 메시지 규격 분석 및 데이터 파싱/처리 로직을 구현했습니다.
        *   **✅ Result:** 안정적인 `OCPP 1.6` 클라이언트를 구현하여 **충전기와 서버 간의 양방향 통신을 구축**하였고, 원격 충전 시스템의 기반을 마련했습니다.

*   **🔧 사용 기술:** `Atmega`, `C++ (Arduino)`, `UART`, `I2C`, `Python`, `Websocket`, `Linux (Ubuntu)`

---

### 🧪 기타 경험 및 연구 (Other Experience)

*   **🖥️ 급속 충전기 테스트용 GUI 개발**
    *   `Python`과 `Tkinter`로 2채널 GUI를 개발하여 **EV TREND KOREA 전시회에서 성공적으로 시연**했습니다.

*   **🚁 드론 통신 테스트 시스템 개발**
    *   `ESP32`와 `LabView`를 활용하여 드론과의 `MAVLink` 통신 프로토콜 연동 및 데이터 추적 시스템을 개발했습니다.

*   **🔬 차세대 GUI 프레임워크 연구**
    *   `Rust` 기반 GUI 프레임워크(Iced,gtk-rs)를 간단하게 구현하여 ARM 프로세서에 적용하고, 성능 및 적용 가능성을 테스트하고 기술 리포트를 작성했습니다.

# 🎓 마이크로프로세서 (Microprocessor & MCU)
> **경희대학교 전자공학과 김동한 교수님 강의 자료실**  
> 본 저장소는 ARM Cortex-M3 코어 기반의 **STM32F103** 마이크로컨트롤러를 이용한 마이크로프로세서 수업의 강의 자료(PDF) 및 STM32CubeIDE 실습 소스코드 패키지를 배포하는 공간입니다.

---

## 📢 과목 및 강사 정보 (Course Information)

| 구분 | 정보 및 링크 |
| :--- | :--- |
| **👨‍🏫 담당 교수** | **김동한 교수** (전자공학과, 전자정보대학 609호, 내선 3831) |
| **✉️ 이메일** | [donghani@khu.ac.kr](mailto:donghani@khu.ac.kr) |
| **⏱️ 상담 시간** | 매주 수업 종료 후 1시간 |
| **📖 주교재** | **STM32CubeIDE를 이용한 STM32 따라하기** (김남수, 이진 저) |
| **🔗 강의 영상** | [YouTube 채널 (경희대 김동한)](https://www.youtube.com/channel/UCT_h-5YhlC0t9LEdVckdrXQ) |
| **💻 실습 포털** | [경희대학교 e-Campus](https://e-campus.khu.ac.kr) |

---

## 📚 주차별 강의 자료 (Lecture Slides)

아래 강의 자료(PDF)는 본 저장소의 루트 디렉토리에 포함되어 있어 즉시 다운로드하거나 확인할 수 있습니다.

| 장 / 주제 | 파일명 (다운로드 링크) | 주요 학습 내용 |
| :--- | :--- | :--- |
| **오리엔테이션** | [0. 마이크로프로세서.pdf](./0.%20%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%ED%94%84%EB%A1%9C%EC%85%8B%EC%96%B4.pdf) <br> [0. 오리엔테이션 및 개발 환경.pdf](./0.%20%EC%98%A4%EB%A6%AC%EC%97%94%ED%85%8C%EC%9D%B4%EC%85%98%20%EB%B0%8F%20%EA%B0%9C%EB%B0%9C%20%ED%99%98%EA%B2%BD%20%EA%B5%AC%EC%84%B1.pdf) | 과목 개요, 평가 방식 및 STM32CubeIDE & ST-LINK 드라이버 설치 가이드 |
| **제1장** | [1. STM32 개요.pdf](./1.%20STM32%20%EA%B0%9C%EC%9A%94.pdf) <br> [1. 기초이론_v2.pdf](./1.%20%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%ED%94%84%EB%A1%9C%EC%85%8B%EC%96%B4%EC%97%90%20%EB%8C%80%ED%95%9C%20%EA%B8%B0%EC%B4%88%EC%9D%B4%EB%A1%A0_v2.pdf) | MCU와 마이크로프로세서 차이, 하바드 vs 폰노이만 구조, STM32F1 시리즈 스펙 |
| **제2장** | [2. ARM Cortex-M 개요.pdf](./2.%20ARM%20Cortex-M%20%ED%94%84%EB%A1%9C%EC%85%8B%EC%96%B4%EC%9D%98%20%EA%B0%9C%EC%9A%94-v2.pdf) <br> [2. STM32 시작하기.pdf](./2.%20STM32%20%EC%8B%DC%EC%9E%91%ED%95%98%EA%B8%B0.pdf) | Cortex-M3 아키텍처, 레지스터 구성, 동작 모드 및 최초의 LED blink 프로젝트 생성 |
| **제3장** | [3. HAL.pdf](./3.%20HAL.pdf) | STM32Cube HAL(Hardware Abstraction Layer) 드라이버 구조 및 API 활용 개요 |
| **제4장** | [4. GPIO & EXTI.pdf](./4.%20GPIO%20%26%20EXIT.pdf) | 범용 입출력(GPIO) 포트 구조, 레지스터 설정 및 외부 인터럽트(EXTI) 우선순위 |
| **제5장** | [5. ADC.pdf](./5.%20ADC.pdf) <br> [5. ARM M3_CH09_ADC.pdf](./5.%20ARM%20M3_CH09_ADC.pdf) | 아날로그-디지털 변환(ADC) 이론, 연속/단일 변환 모드 및 가변저항 센서 리딩 |
| **제6장** | [6. TIM.pdf](./6.%20TIM.pdf) <br> [6. 타이머를 이용한 입출력 제어.pdf](./6.%20ARM%20M3_CH08_%ED%83%80%EC%9D%B4%EB%A8%B8%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EC%9e%85%EC%B6%9c%EB%A0%A5%20%EC%A0%9C%EC%96%B4.pdf) | 타이머(Timer) 구조, 카운터 모드, PWM 출력 생성 및 RGB LED, RC 서보모터 제어 |
| **제7장** | [7. Serial Communication.pdf](./7.%20Serial%20Communication.pdf) <br> [7-2. I2C 통신.pdf](./7-2.%20I2C%20%ED%86%B5%EC%8B%A0.pdf) | 직렬 통신 기법(UART, I2C, SPI)의 비교 분석 및 인터럽트 방식(IT)의 통신 처리 |

---

## 🛠️ STM32F103 실습 소스코드 패키지 (`/STM32F103`)

STM32CubeIDE로 즉시 임포트(Import)하여 빌드 및 디버깅할 수 있도록 정돈된 공식 수업용 프로젝트 모음입니다.

### 💡 **구현 카테고리별 프로젝트 목록**

#### 🟢 **1. 기본 입출력 및 디버깅 (GPIO & Debug)**
* **[2. LED_Blink](./STM32F103/2.%20LED_Blink):** 가장 기본적인 LED 점멸 제어 (HAL_GPIO_TogglePin)
* **[2. Serial Debug](./STM32F103/2.%20Serial%20Debug):** `printf` 함수를 UART로 리다이렉션하여 시리얼 디버깅 환경 구축
* **[4. GPIO_Basic](./STM32F103/4.%20GPIO_Basic) / [EVB1](./STM32F103/4.%20GPIO_EVB1) / [EVB2](./STM32F103/4.%20GPIO_EVB2):** 스위치 입력을 받아 LED를 제어하는 GPIO 입출력 실습

#### 🟡 **2. 외부 인터럽트 (External Interrupt - EXTI)**
* **[4. EXTI_Basic](./STM32F103/4.%20EXTI_Basic) / [EVB1](./STM32F103/4.%20EXIT_EVB1) / [EVB2](./STM32F103/4.%20EXTI_EVB2) / [EVB3](./STM32F103/4.%20EXTI_EVB3):** 푸시 버튼 입력을 하드웨어 외부 인터럽트로 트리거하여 실시간 콜백함수 처리 구현

#### 🟠 **3. 아날로그 변환 및 센싱 (ADC)**
* **[5. ADC_Basic](./STM32F103/5.%20ADC_Basic) / [EVB1](./STM32F103/5.%20ADC_EVB1) / [EVB2](./STM32F103/5.%20ADC_EVB2):** ADC 단일 채널 및 다중 채널 폴링(Polling) 방식 가변저항 센서 전압 측정

#### 🔵 **4. 타이머 및 제어 기법 (Timer, PWM & Motor)**
* **[6. TIM_Basic](./STM32F103/6.%20TIM_Basic):** 타이머 업데이트 오버플로우 인터럽트를 이용한 정확한 주기적 시간 제어
* **[6. TIM_PWM](./STM32F103/6.%20TIM_PWM):** 펄스 폭 변조(PWM) 파형 생성 및 듀티비 조절
* **[6. TIM_Buzzer](./STM32F103/6.%20TIM_Buzzer):** PWM 주파수를 가변하여 수동 부저(Buzzer) 멜로디 연주
* **[6. TIM_RGB-LED](./STM32F103/6.%20TIM_RGB-LED):** 3채널 PWM을 활용한 RGB LED 컬러 믹싱 제어
* **[6. TIM_Servo](./STM32F103/6.%20TIM_Servo):** $20\text{ms}$ 주기와 $1\text{ms}\sim2\text{ms}$ 펄스를 이용한 RC 서보모터(Servo) 각도 제어

#### 🟣 **5. 직렬 통신 프로토콜 (Serial Communication)**
* **[7. Serial-Comm_UART](./STM32F103/7.%20Serial-Comm_UART):** 기본적인 UART 문자열 송수신 (Polling 방식)
* **[7. Serial-Comm_UART-IT](./STM32F103/7.%20Serial-Comm_UART-IT):** 수신 인터럽트(RXNE)를 이용한 비차단식 안정적 시리얼 통신
* **[7. Serial-Comm_I2C](./STM32F103/7.%20Serial-Comm_I2C):** I2C 프로토콜을 이용한 슬레이브 디바이스 제어 기초

#### ⚙️ **6. 외부 디바이스 & 드라이버 (Extra Peripherals)**
* **[Extra. CLCD](./STM32F103/Extra.%20CLCD):** 8비트/4비트 인터페이스 방식의 캐릭터 LCD(HD44780) 글자 출력 제어
* **[Extra. EEPROM](./STM32F103/Extra.%20EEPROM) / [at24c](./STM32F103/at24c):** I2C 통신 기반의 AT24C 계열 비휘발성 EEPROM 데이터 쓰기/읽기 드라이버 구현
* **[Extra. HC-SR04](./STM32F103/Extra.%20HC-SR04):** 에코 핀의 에코 펄스 하이 구간 시간을 타이머로 측정하는 초음파 거리 센서 정밀 제어

---

## 🚀 빠른 시작 가이드 (Quick Start)

### 1. STM32CubeIDE로 프로젝트 불러오기
1. **STM32CubeIDE**를 실행합니다.
2. 상단 메뉴에서 **File ➔ Import...**를 선택합니다.
3. **General ➔ Existing Projects into Workspace**를 선택하고 **Next**를 누릅니다.
4. **Select root directory** 옆의 **Browse...** 버튼을 클릭하여 본 저장소 내 `STM32F103/` 폴더 아래 원하는 예제 폴더(예: `2. LED_Blink`)를 선택합니다.
5. **Projects** 목록에 프로젝트명이 뜨면 체크 후 **Finish**를 클릭합니다.

### 2. 빌드 및 디버깅
1. MCU 보드(예: STM32F103 개발 보드)를 **ST-LINK** 디버거를 통해 PC와 연결합니다.
2. 상단 툴바의 **Build** 망치 아이콘(또는 `Ctrl+B`)을 눌러 프로젝트를 빌드합니다.
3. **Debug** 벌레 아이콘을 눌러 MCU에 펌웨어를 다운로드하고, 실시간 라인 브레이크포인트 디버깅을 실행합니다.

# 🌐 경희대학교 마이크로프로세서 강의자료실 (Class Microprocessor)

Welcome! 본 사이트는 경희대학교 전자공학과 김동한 교수님의 **마이크로프로세서(Microprocessor & MCU)** 과목 강의자료실입니다.
교재(STM32CubeIDE를 이용한 STM32 따라하기)와 관련된 이론 강의 자료(PDF) 및 ARM Cortex-M3 기반의 **STM32F103** MCU용 수업용 매트랩 실습 및 STM32CubeIDE 소스코드 패키지를 배포하고 있습니다.

---

## 👨‍🏫 강사 및 교과 정보 (Course Overview)

* **강사:** 전자공학과 김동한 교수 (전자정보대학 609호)
* **연락처:** donghani@khu.ac.kr | 내선번호 3831
* **상담시간:** 수업 후 1시간
* **주교재:** **STM32CubeIDE를 이용한 STM32 따라하기** (김남수, 이진 저)
* **보조자료:** [유튜브 강의 채널 (경희대 김동한)](https://www.youtube.com/channel/UCT_h-5YhlC0t9LEdVckdrXQ)
* **강의 업로드:** [경희대학교 e-Campus](https://e-campus.khu.ac.kr) 및 본 GitHub 저장소

---

## 📚 1. 주차별 이론 강의 교안 (Lecture Slides)

각 단원 번호를 클릭하여 다운로드할 수 있습니다.

* 📢 [**0. 마이크로프로세서 과목 소개**](./0.%20%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%ED%94%84%EB%A1%9C%EC%85%8B%EC%96%B4.pdf)
  * 과목 운영 방식 및 MCU 개발 환경 구축 요령
* 💻 [**0. 오리엔테이션 및 개발 환경 구성**](./0.%20%EC%98%A4%EB%A6%AC%EC%97%94%ED%85%8C%EC%9D%B4%EC%85%98%20%EB%B0%8F%20%EA%B0%9C%EB%B0%9C%20%ED%99%98%EA%B2%BD%20%EA%B5%AC%EC%84%B1.pdf)
  * STM32CubeIDE 및 ST-Link 드라이버 상세 설치
* 📖 [**1. STM32 개요 및 마이크로프로세서 기초**](./1.%20STM32%20%EA%B0%9C%EC%9A%94.pdf) & [**기초이론 v2**](./1.%20%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%ED%94%84%EB%A1%9C%EC%85%8B%EC%96%B4%EC%97%90%20%EB%8C%80%ED%95%9C%20%EA%B8%B0%EC%B4%88%EC%9D%B4%EB%A1%A0_v2.pdf)
  * CPU, Microcontroller, Microprocessor 역사, Harvard Architecture 스펙
* 📖 [**2. ARM Cortex-M 프로세서 개요**](./2.%20ARM%20Cortex-M%20%ED%94%84%EB%A1%9C%EC%85%8B%EC%96%B4%20%EA%B0%9C%EC%9A%94-v2.pdf) & [**STM32 시작하기**](./2.%20STM32%20%EC%8B%DC%EC%9E%91%ED%95%98%EA%B8%B0.pdf)
  * Cortex-M3 아키텍처 특성, 레지스터 구조 및 최초의 LED Blink 코딩
* 📖 [**3. HAL (Hardware Abstraction Layer)**](./3.%20HAL.pdf)
  * 로우 레벨 레지스터 제어 대비 HAL 드라이버 설계 구조 및 HAL API 활용법
* 📖 [**4. GPIO & EXTI (입출력 및 외부 인터럽트)**](./4.%20GPIO%20%26%20EXIT.pdf)
  * 입출력 핀 구성, 속도 조절, 풀업/풀다운 및 EXTI 인터럽트 벡터 처리
* 📖 [**5. ADC (Analog-Digital Converter)**](./5.%20ADC.pdf) & [**ARM M3 ADC 상세**](./5.%20ARM%20M3_CH09_ADC.pdf)
  * 아날로그 센서 데이터 수집을 위한 분해능 및 스캐닝, DMA 연결성
* 📖 [**6. TIM (Timer & Counter)**](./6.%20TIM.pdf) & [**타이머 제어 상세**](./6.%20ARM%20M3_CH08_%ED%83%80%EC%9D%B4%EB%A8%B8%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EC%9e%85%EC%B6%9c%EB%A0%A5%20%EC%A0%9C%EC%96%B4.pdf)
  * 타이머 주파수 설정, 분주기(Prescaler) 연산, PWM 주파수/듀티비, 부저음 합성 및 서보 제어
* 📖 [**7. Serial Communication (직렬 통신)**](./7.%20Serial%20Communication.pdf) & [**I2C 통신**](./7-2.%20I2C%20%ED%86%B5%EC%8B%A0.pdf) & [**업데이트본**](./7.%20Serial%20Communication-updated.pdf)
  * UART 비차단 IT 통신, I2C 버스 주소 제어 및 AT24C EEPROM 인터페이스

---

## 🛠️ 2. STM32F103 공식 수업 실습 소스코드

MCU 하드웨어를 직접 코드로 움직이는 실습 예제 디렉토리 구조입니다.

### 🟢 1. 기본 입출력 및 디버깅 (GPIO & Debug)
* [**2. LED_Blink**](./STM32F103/2.%20LED_Blink): LED 점등 및 점멸 (HAL_GPIO_TogglePin)
* [**2. Serial Debug**](./STM32F103/2.%20Serial%20Debug): UART를 이용한 printf 시리얼 디버그 출력 터미널 구축
* [**4. GPIO_Basic / EVB1 / EVB2**](./STM32F103/4.%20GPIO_Basic): 푸시 스위치 입력 인식 및 LED 출력 연동

### 🟡 2. 외부 인터럽트 (EXTI)
* [**4. EXTI_Basic / EVB1 / EVB2 / EVB3**](./STM32F103/4.%20EXTI_Basic): 스위치 바운싱 제거 및 하드웨어 외부 인터럽트 콜백 처리

### 🟠 3. 아날로그 센싱 (ADC)
* [**5. ADC_Basic / EVB1 / EVB2**](./STM32F103/5.%20ADC_Basic): 가변저항 전압 폴링 채널 획득

### 🔵 4. 타이머 및 액추에이터 제어 (TIM, PWM, Servo)
* [**6. TIM_Basic**](./STM32F103/6.%20TIM_Basic): 타이머 카운트 인터럽트를 이용한 주기 동작
* [**6. TIM_PWM**](./STM32F103/6.%20TIM_PWM): PWM 파형 생성 및 타이머 레지스터 CCR 설정
* [**6. TIM_Buzzer**](./STM32F103/6.%20TIM_Buzzer): 부저 주파수 멜로디 믹싱
* [**6. TIM_RGB-LED**](./STM32F103/6.%20TIM_RGB-LED): RGB LED 컬러 제어
* [**6. TIM_Servo**](./STM32F103/6.%20TIM_Servo): $20\text{ms}$ 주기 PWM 신호 기반 RC 서보 모터 제어

### 🟣 5. 시리얼 버스 통신 (UART & I2C)
* [**7. Serial-Comm_UART / UART-IT**](./STM32F103/7.%20Serial-Comm_UART): UART 인터럽트 방식 송수신
* [**7. Serial-Comm_I2C**](./STM32F103/7.%20Serial-Comm_I2C): I2C 통신 프로토콜을 이용한 디바이스 제어

### ⚙️ 6. 외장 모듈 활용 (Extra)
* [**Extra. CLCD**](./STM32F103/Extra.%20CLCD): 캐릭터 LCD 디스플레이 문자 출력 드라이버
* [**Extra. EEPROM & at24c**](./STM32F103/Extra.%20EEPROM): I2C 기반 비휘발성 AT24C EEPROM 바이트 단위 데이터 저장
* [**Extra. HC-SR04**](./STM32F103/Extra.%20HC-SR04): 초음파 거리 센서 트리거 및 에코 타임 측정

---

## 🚀 STM32CubeIDE 프로젝트 임포트 가이드

1. **STM32CubeIDE** 실행 후 **File > Import...** 진입
2. **General > Existing Projects into Workspace** 선택 후 **Next**
3. `STM32F103/` 디렉토리 아래의 실습 프로젝트 폴더를 선택하고 **Finish**
4. 프로젝트 선택 후 **Ctrl + B**로 빌드, **ST-LINK** 디버거를 연결하여 **Debug** 실행

# 🌿 Welcome to 4iren (4팀)

> **공간 융합형 데이터 기반 AIoT 지능형 강의실 환경 제어 플랫폼**
> 10주간 함께 만들어가는 인공지능 기반 환경 관리 솔루션

## 📌 Project Overview
교육 시설마다 다른 강의실의 구조적 특성(크기, 창문, 단열 등)과 유동적인 재실 상태를 반영하여, 기존의 일률적인 환경 제어(Rule-based) 규칙이 가진 한계를 혁신합니다.

외부 날씨 API와 실내 환경 센서(온·습도, 기압, CO2, 도어) 데이터를 융합해 LLM이 맥락 인지형 제어 가이드를 제공합니다. 또한, 공간별 하드웨어 특성과 사용자 집단의 행동 패턴을 머신러닝(ML)으로 학습하여 별도의 초기 세팅 없이 플러그앤플레이(Plug & Play) 형태로 즉시 도입 가능한 상용 AIoT 솔루션을 구축하는 것을 목표로 합니다.

## 🚀 Key Features
* **LLM 컨텍스트 인식 & 웰컴 브리핑:** 매일 아침 도어 센서 첫 개방 시, 당일 날씨와 실내 공기질을 종합하여 직관적인 웰컴 브리핑 텍스트 알림 및 자연어 기반 제어 가이드 제공.
* **멀티모달 시계열 기반 정밀 재실 분석 & 대시보드:** 도어 센서 이벤트와 CO2 농도의 기울기(Gradient)를 분석해 빈 공간을 정밀하게 구분하여 에너지 관리(BEMS) 자동화 및 관리자용 모니터링 대시보드 지원.
* **공간 도메인 적응 & 집단 맞춤형 학습 (ML):** 각 강의실의 물리적 고유 특성과 사용자 피드백을 누적 학습하여 스스로 최적의 쾌적 지표를 도출하고, 이를 룰 엔진과 연동해 자동 대응.
* **Fault Tolerance (센서 이상 탐지):** 통계적 알고리즘을 통해 센서 노이즈나 고정 에러(Stuck) 등을 실시간으로 필터링하여 시스템 오작동 방지.
* **안정적인 아키텍처 및 파이프라인:** JWT 기반 인증 체계와 MSA 구조를 도입하고, TSDB와 RDB를 병행하여 대용량 센서 데이터를 안정적으로 수집/가공하는 파이프라인 구축.

## 👨‍💻 Team Members

| 이름 | 포지션 / 역할 |                       GitHub                       |
| :---: | :---: |:--------------------------------------------------:|
| **김태희** | Frontend / 대시보드 UI 구현 |         [@pp0ng](https://github.com/pp0ng)         |
| **신준식** | AI / 머신러닝 공간 도메인 학습 |    [@shinjunsik](https://github.com/shinjunsik)    |
| **윤채영** | Backend / JWT 인증 및 사용자 관리 |     [@yooncy123](https://github.com/yooncy123)     |
| **유대연** | IoT / 센서 연동 및 이상 탐지 알고리즘 |        [@Uoo-uu](https://github.com/Uoo-uu)        |
| **이정민** | Data / TSDB+RDB 병행 설계 및 데이터 가공 |    [@jeongmin26](https://github.com/jeongmin26)    |
| **전유진** | Backend / Spring Boot 기반 MSA 설계 및 통합 |        [@onyune](https://github.com/onyune)        |
| **최이건** | AI / LLM 연동 및 프롬프트 처리 모듈 | [@likeironbasic](https://github.com/likeironbasic) |
| **황지원** | Infra / CI·CD 및 고가용성 아키텍처 배포 |     [@hjiwon203](https://github.com/hjiwon203)     |
| **전재나** | Data / RabbitMQ 룰 엔진 및 메시지 브로커 |      [@JAENA216](https://github.com/JAENA216)      |

## 🛠️ Architecture & Tech Stack
* **Backend:** Spring Boot 기반 MSA(마이크로서비스 아키텍처)
* **Message Broker:** RabbitMQ / Kafka (센서 데이터 비동기 수집)
* **Data & AI:** Elasticsearch (시계열 검색), TSDB + RDB 병행 아키텍처
* **Infra:** 이중화 기반 무중단 고가용성 구조

## 🤝 Ground Rules
* **일일 미팅:** 매일 오전 9시 (어제 한 일, 오늘 할 일, 이슈 공유)
* **일일 커밋:** 매일 오후, 진행 상황을 알 수 있도록 명확한 커밋 메시지와 함께 PUSH
* **주간 미팅:** 주 1회 멘토 점검 및 주간 스프린트 회고
* **상호 평가:** 프로젝트 초, 중, 후반 총 3회에 걸쳐 팀원 상호 피드백 진행
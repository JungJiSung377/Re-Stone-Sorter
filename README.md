# 💎 Re-Stone Sorter: AI-Powered Automated Mineral Sorting System
> **딥러닝 기반 유해 광물 자동 선별 및 자원 회수 최적화 시스템**

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?logo=PyTorch&logoColor=white)](https://pytorch.org/)
[![Hardware](https://img.shields.io/badge/Hardware-Air--Jet%20Ejector-orange)](https://github.com/JungJiSung377/ReStone-Sorter)
[![ESG](https://img.shields.io/badge/ESG-Environmental%20Protection-green)](https://www.env.go.kr/)

본 프로젝트는 강원도 폐광 지역의 경석(폐석) 문제를 해결하기 위해 **AI 비전 기술**과 **에어 젯(Air-Jet) 선별기**를 결합한 자동화 시스템입니다. 파분쇄 공정 전 유해 광물을 사전에 선별하여 에너지 효율을 극대화하고 환경 오염을 원천 차단합니다.

---

## 📝 01. 요약 (Abstract)
> 기존의 광물 분석은 고비용의 XRF 분석이나 수동 선별에 의존하여 효율이 낮았습니다. **Re-Stone Sorter**는 컨베이어 벨트 위의 암석을 실시간으로 전수 조사하며, 특히 전체 공정 에너지의 50% 이상이 소모되는 파분쇄 단계 이전에 맥석을 제거함으로써 **약 40%의 에너지 절감**과 **60%의 비용 절감** 효과를 제공합니다.

---

## 🛠️ 02. 시스템 아키텍처 (System Architecture)
본 시스템은 인지(Perception)와 제어(Actuation)가 결합된 통합 솔루션입니다.

### 1. Hardware: Vision Box & Air-Jet Ejector
* **AI Vision Box:** 고속 카메라와 조명 시스템을 통해 이동하는 광물의 시각 데이터를 실시간 수집합니다.
* **Air-Jet Ejector:** AI가 판별한 유해 광물의 위치에 정밀하게 공기를 분사하여 물리적으로 분리합니다.

### 2. Software: SAM-YOLO Pipeline
* **SAM (Segment Anything Model):** 다양한 암석의 형태를 정밀하게 마스킹하여 객체 경계를 확정합니다.
* **YOLO (You Only Look Once):** 실시간으로 광물의 종류(황철석, 경석 등)를 초고속 분류합니다.

---

## 🔄 03. 전체 공정 흐름 (Process Workflow)
광산 현장의 기존 공정에 유기적으로 통합되어 운영 효율을 높입니다.

| 단계 | 공정 명칭 | 역할 및 특징 |
| :--- | :--- | :--- |
| **Step 1** | **1차 파쇄 (Jaw Crusher)** | 원석을 선별 가능한 크기로 파쇄 |
| **Step 2** | **Re-Stone Sorter** | **AI 비전 판별 및 에어 젯 선별 (핵심 구간)** |
| **Step 3** | **분쇄 (Ball Mill)** | 선별된 유가 광물만 집중 분쇄 (에너지 절감) |
| **Step 4** | **최종 제품화** | 부유 선별 및 제련을 통한 자원 회수 |

---

## 🔬 04. 기술적 차별점 (Technical Breakthrough)
* **에너지 효율 최적화:** 파분쇄 공정 유입 물량을 사전 차단하여 공정 부하를 획기적으로 감소시킵니다.
    * $$E_{saved} \approx 40\% \quad \text{(Total Comminution Energy)}$$
* **실시간 전수 조사:** 표본 추출 방식의 한계를 극복하고 벨트 위 모든 암석을 실시간 스캔합니다.
* **환경 오염 원천 차단:** 산성 광산 배수(AMD)의 주원인인 황철석 등을 파쇄 전 원형 상태로 제거합니다.

---

## ✅ 05. 기대 가치 (Impact & ESG)
* **경제적 가치:** 고비용 XRF 분석을 저비용 AI 비전으로 대체하여 경제적 타당성 확보.
* **환경적 가치:** 토양 및 수질 오염 예방 및 생산 톤당 탄소 배출량 감소.
* **사회적 가치:** 폐광 지역의 환경 문제 해결 및 새로운 자원 순환 생태계 구축.

---

## 📚 06. 참고문헌 (References)
* [1] Ballantyne et al., "Proportion of energy attributable to comminution," *The Weir Group*, 2012.
* [2] 이계승, 전효택, "태백산 광화대 선탄경석의 광물학적 특성," *한국자원공학회지*, 2010.
* [3] 강원테크노파크, "강원도 석탄 경석 활용 산업화 방안 보고서," 2023.

---

## 🧑‍💻 Contributors
* **정지성 (Jisung Jung)** - 에너지자원공학과 (AI 모델 설계 및 데이터 분석)
* **설재훈 (Jaehoon Seol)** - 메카트로닉스공학과 (하드웨어 제어 및 시스템 통합)
* **Affiliation:** 강원대학교 융합소프트웨어랩 (Convergence Software Lab)


### 모델 구현 및 검증 데이터

![모델 구현 이미](https://github.com/JungJiSung377/Re-Stone-Sorter/blob/main/image.png)





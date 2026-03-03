# 📌 금융 IT 관점에서의 MSA 아키텍처 설계와 운영 전략

- 우리FISA 1차 기술세미나  
- 팀: 돈지켜조
- 주제: 금융권 MSA 도입 전략 및 우리은행 적용 제안
  
| **우민하** | **김동환** | **최예원** | **심효진** |
|---|---|---|---|
| • MSA 개요 정리 <br> • 모놀리식 vs MSA 비교 분석 | • MSA 도입 유의사항 분석 <br> • 도입 실패 사례 | • 금융권 MSA 도입 사례 분석 <br> • 코어뱅킹 아키텍처 구조 연구 | • 우리은행 관점 MSA 파일럿 전략 제안 <br> • 통신 MSA 아키텍쳐 설계 |

  

<img width="1920" height="1080" alt="30" src="https://github.com/user-attachments/assets/e8e68b77-1831-4b71-a44c-ab679589feca" />

<img width="1920" height="1080" alt="32" src="https://github.com/user-attachments/assets/96a56eb1-16f1-4f74-aaf7-40a750592724" />

<img width="1920" height="1080" alt="33" src="https://github.com/user-attachments/assets/5d2152b2-da64-4f55-9c07-5fa4cb44d989" />



## 💡 Why


본 세미나는 단순히 MSA 개념을 설명하는 것이 아니라,  
**금융권 환경에서 MSA를 어떻게 현실적으로 도입할 것인가**에 대한 전략적 접근을 목표로 하였음.

- 강한 ACID 정합성
- 초저지연 OLTP 환경
- 대규모 레거시 시스템
- 절대 장애가 허용되지 않는 구조

> 금융권에서 MSA는 “가능한가?”가 아니라  “어떻게 도입해야 안전한가?”

---

## 🔍 What We Did

- 전통적 코어뱅킹 아키텍처 분석
- 국내 MSA 전환 사례(토스뱅크) 구조 연구
- 분산 트랜잭션 / 정합성 전략 분석
- 분산 모놀리식 위험 검토
- 우리은행 환경에 맞는 도입 시나리오 설계

---

## 🎯 Our Conclusion

코어를 한 번에 바꾸는 것은 현실적이지 않음.

제안사항: 채널계 파일럿 → 검증 체계 확보 → 점진적 확산
파일럿 대상으로 통신(MVNO) 모바일 사업을 선정.

고려사항: 정합성 리스크 및 계정계 결합도

---

## 📌 Feedback
### ✅ Strengths

- 금융 산업 특수성(규제, 가용성, 보안, 감사, 트랜잭션 무결성)을 잘 반영한 설계
- 코어뱅킹 및 계정계 시스템의 운영 중심 구조에 대한 현실적 이해
- 토스뱅크 사례를 단순 조사 수준이 아닌, 우리은행에 적용 가능한 구조적 제안으로 발전시킴
- 실제 솔루션 아키텍트 제안과 유사한 설득력 있는 발표 구성
- MSA 도입 필요성과 배경 설명이 논리적으로 타당함

---

### 🏦 Financial IT Insights

- 시중은행은 시스템 변경에 매우 보수적
- 코어뱅킹은 개발보다 운영 비중이 높음 (안정성 최우선)
- 계정계 데이터는 은행의 원천 데이터로:
  - 시스템 중단 불가
  - 레이턴시 최소화 필수
  - 데이터 무결성 보장 필수
- 계정계 아키텍처 변경은 보통 차세대(10년 단위) 프로젝트 수준에서 진행

---

### ⚠️ Improvements

####  Technical Term Explanation

- ACID, MSA, OLTP, Saga, Strangler Pattern, FINOS, DLQ, BFF 등  
  전문 용어 사용 시 최초 등장 지점에서 정의 및 약어 설명 필요
- 개념 → 정의 → 적용 흐름으로 재구성 필요

![질의응답](https://github.com/user-attachments/assets/a10758b9-f1c9-454f-998c-3d77dccbbf0b)


[우리FISA - 돈지켜줘 금융MSA도입전략.pdf](https://github.com/user-attachments/files/25566990/FISA.-.MSA.pdf)

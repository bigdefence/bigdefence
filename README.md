<div align="center">

# 정강빈 (Kangbin Jeong)
### 🤖 Multimodal AI Engineer | LLM Specialist

[![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=bigdefence)](https://solved.ac/bigdefence)
[![GitHub followers](https://img.shields.io/github/followers/bigdefence?style=social)](https://github.com/bigdefence)
[![HuggingFace](https://img.shields.io/badge/🤗_HuggingFace-1500+_downloads-yellow)](https://huggingface.co/bigdefence)

</div>

---

## 👨‍💻 About Me

> **"보고 듣고 말하는 AI"** - 멀티모달 AI로 세상과 소통하는 미래를 만듭니다.

**Vision-Language Model (VLM)** 과 **Audio LLM** 개발에 특화된 AI 엔지니어입니다.  
자체 개발한 한국어 멀티모달 모델을 오픈소스로 공개하며, 실시간 대화 시스템 구축 경험을 보유하고 있습니다.

### 🎯 핵심 강점
- ✅ **자체 VLM 개발**: Vision Encoder + LLM 통합, 2단계 학습 전략 (Pretrain → LoRA Finetune)
- ✅ **Audio LLM 전문**: Speech Encoder + LLM, 4개 한국어 LLM 백본 호환 시스템 구축
- ✅ **실시간 파이프라인**: STT → VLM → Streaming TTS, 저지연 멀티모달 대화 구현
- ✅ **오픈소스 기여**: HuggingFace 1,500+ 다운로드, Apache 2.0 라이선스 공개
- ✅ **복구 회복력 설계**: 임베딩 차원 불일치 자동 감지 및 인덱스 재생성 등 실무 문제 해결

---

## 🛠️ Tech Stack

<table>
<tr>
<td width="50%" valign="top">

### 🧠 AI/ML
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=PyTorch&logoColor=white)
![Transformers](https://img.shields.io/badge/🤗_Transformers-FFD21E?style=flat-square)
![LangChain](https://img.shields.io/badge/🦜_LangChain-121212?style=flat-square)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=OpenCV&logoColor=white)

### 🎙️ Multimodal AI
- **Vision**: CLIP, Vision Transformer, MediaPipe
- **Audio**: Whisper, CosyVoice2, OpenAI TTS
- **LLM**: LLaMA, EXAONE, Gemini, ChatGPT

</td>
<td width="50%" valign="top">

### 💻 Development
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=FastAPI&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=Flask&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

### ☁️ Cloud & Tools
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=google-cloud&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Weights & Biases](https://img.shields.io/badge/W&B-FFBE00?style=flat-square&logo=weightsandbiases&logoColor=black)

</td>
</tr>
</table>

---

## 📊 Key Achievements

<div align="center">

| 🎯 Metric | 📈 Achievement |
|:---:|:---:|
| **🏆 수상** | 최우수상 🥇, 우수상 🥈 × 2 |
| **📦 오픈소스** | HuggingFace 1,500+ 다운로드 |
| **💡 프로젝트** | 21+ AI 프로젝트 개발·배포 |
| **🔬 모델 개발** | VLM·Audio LLM 자체 개발 |

</div>

---

## 🏆 Featured Projects

### 🐟 Neofish — 차세대 AI 예측 엔진 및 집단지성 시뮬레이션 플랫폼
**2026.03 - 현재** | [Repo](https://github.com/bigdefence/Neofish)

[![Neofish Demo](https://img.youtube.com/vi/lKeVcfvjavs/maxresdefault.jpg)](https://youtu.be/lKeVcfvjavs)

> 정적인 문서 분석을 넘어, 현실 세계의 정보와 이해관계자들의 비합리적 심리 요소를 가상 소셜 공간에 투영하여 미래 시나리오를 예측·예방하는 **엔드투엔드 멀티 에이전트 시뮬레이션 플랫폼**입니다.

**🎯 핵심 기능 및 특장점**
- ✅ **하이브리드 Graph RAG (3072 dim)**: Gemini 2.0 임베딩 기반 벡터 검색, Neo4j 검색, 키워드 매칭을 결합하여 정확도를 극대화
- ✅ **시스템 회복력 (Auto-Recovery)**: 임베딩 모델 교체 시 Neo4j 벡터 인덱스 차원 불일치를 자동 감지하고 즉시 재생성하는 안정적인 복구 파이프라인 구축
- ✅ **심리 시뮬레이션 레이어 (Human Factors)**: 에이전트에게 **Big Five 인격 모델** 및 10여 종의 **인지 편향**을 주입하고, 전역 환경 변수(동조 압력, 감정 전염 속도)를 통해 현실적인 군중 심리 재현
- ✅ **벡터 기반 고속 엔터티 해상도 (Entity Resolution)**: **Numpy/Scikit-learn**을 활용한 고속 코사인 유사도 연산으로 병합 후보를 선별하여 LLM 호출 비용 절감 및 그래프 구축 속도 획기적 개선
- ✅ **OASIS(CAMEL-AI) 병렬 시뮬레이션**: Twitter / Reddit 병렬 모드로 집단 행동을 재현하며, **subprocess**와 **파일 기반 IPC**를 통해 웹 서버와 시뮬레이션 엔진 간의 안정적인 비동기 협업 구현
- ✅ **이중 LLM 전략 및 ReAct 패턴**: 경량 모델(대량 호출)과 고급 추론 모델(온톨로지/분석)을 분리 매핑하고, **ReportAgent**가 ReAct 루프를 통해 자율적으로 그래프 지식을 탐색 및 리포트 생성
- ✅ **멀티미디어 확장 (AI 팟캐스트)**: 보고서 마크다운을 분석하여 Gemini TTS 기반의 2인 패널 대화형 오디오 콘텐츠 자동 생성
- ✅ **D3.js 관계 네트워크 UI**: 의미 검색·줌·이웃 강조 기능이 포함된 대화형 그래프 시각화로 복잡한 지식 구조 탐색성 강화 (Vue 3)

**🔧 기술적 구현 및 시스템 아키텍처**
- **데이터 최적화**: Neo4j 5.x의 Vector Index와 Full-Text Index를 하이브리드로 운용하여 대규모 지식 구조에서도 밀리초 단위의 시맨틱 조회 보장
- **심리 엔진 설계**: `WorldPsychologyConfig`를 통한 집단 역학 시뮬레이션 및 에이전트별 `Emotional Reactivity` 활동 제어 로직 구현
- **Frontend / Backend**: Vue 3 · D3 · Python FastAPI · Neo4j Bolt · OASIS (CAMEL-AI) · Numpy · Scikit-learn · Google GenAI (Embedding/TTS)

---

### 📈 주식의 방 — AI 멀티에이전트 주식 토론 분석 플랫폼
**2026.03 - 현재** | [Demo](https://stockrooms.site/)

[![주식의 방 Demo](https://img.youtube.com/vi/heKGrK1Q0-E/maxresdefault.jpg)](https://www.youtube.com/watch?v=heKGrK1Q0-E)

> 실시간 웹 검색 데이터를 기반으로 4명의 전문 AI 에이전트가 토론·분석하여 종합 투자 인사이트를 제공하는 **멀티 에이전트 주식 토론 플랫폼**

**🤖 Council of Four 에이전트**
| 에이전트 | 역할 | 전문 영역 |
|:---:|:---|:---|
| 📰 **Lyra** | 시장 심리·미디어 분석가 | 뉴스 센티먼트, Fear & Greed, 내러티브 흐름 |
| 📊 **Orion** | 퀀트·기술적 분석가 | 차트 지표, 수급, 섹터 로테이션, 펀더멘털 |
| ⚠️ **Nemesis** | 리스크·역발상 분석가 | 매크로 리스크, 블랙스완, 백테스팅 리스크 매핑 |
| 🎯 **Apex** | 수석 투자 전략가 | 최종 포지션 권고 (매수/매도/관망) |

**🎯 핵심 기능 및 특장점**
- ✅ **LLM 의도 파악 & 4-Agent 토론**: Rule-based를 탈피한 범용 LLM Intent 파악 처리 및 4 에이전트 다각도 토론
- ✅ **선제적 AI 능동 모드 (Proactive Mode)**: 사용자의 단편적 질문에도 AI가 스스로 심층 후속 분석 방향을 제안하고 자율 분석(Deep Dive) 수행
- ✅ **다중 쿼리 동적 검색 시스템**: 뉴스, 리스크, 시세 등 쿼리를 동시 자동 생성 및 출처(Citation) 인용으로 신뢰성 대폭 향상
- ✅ **시각적 에이전트 애니메이션**: 상태(대기/탐색/분석 등)에 따라 실시간 반응하는 픽셀 아트 애니메이션(Pixel Agent)을 제공해 작업 시각화
- ✅ **프리미엄 UI & 실시간 렌더링**: Glassmorphism 기반 UI 고도화, FastAPI SSE를 통한 저지연 초고속 스트리밍 UX

**🔧 기술적 구현**
- **기능 모듈화**: 책임 분리(Separation of Concerns) 원칙에 따른 백엔드 모듈 최적화 및 유지보수성 확보
- **AI / Data Pipeline**: Gemini API (Intent & Generation), Tavily (Search), yfinance (Market Data)
- **Frontend / Backend**: React 18, TypeScript, Vite, Supabase / FastAPI, SSE Network Tuning

---

### 🎨 Magic Canvas: AI 기반 컨텍스트 인식 디자인 에이전트
**2025.11 - 현재** | [Magic Canvas](https://magiccanvas.co.kr/)

[![Magic Canvas Demo](https://img.youtube.com/vi/5pb4txbwxJ8/maxresdefault.jpg)](https://youtu.be/5pb4txbwxJ8)

> 캔버스 위에서 이미지, 텍스트, 드로잉을 조합하면 AI가 시각적 의도를 파악하여 고품질 광고 소재를 자동 생성하는 **차세대 멀티모달 프롬프트리스 디자인 툴**

**🎯 핵심 기능 및 특장점**
- ✅ **시각적 의도 해석**: Gemini 활용 캔버스 스냅샷 및 사용자 드로잉(화살표, 여백 등) 문맥의 복합적 분석
- ✅ **객체 단위 관계 매핑**: 화면 내 요소들의 공간적 관계와 흐름을 분석하여 이상적인 생성 프롬프트 자동 도출
- ✅ **5대 특화 AI 생성 도구**: 스마트 배경 생성, 배경 제거, 광고 배너 팩토리, 상세페이지 섹션화, 텍스트 리터칭 통합
- ✅ **다이내믹 멀티 모델 파이프라인**: 작업 목적에 맞춰 최적의 이미지/영상 생성 모델 앙상블 적용

**🛠️ 기술 스택**
- **Frontend**: React 18, Fabric.js (Canvas API), Framer Motion, Zustand
- **Backend**: FastAPI, 비동기 파이프라인(`asyncio`), Pillow
- **Infra**: Supabase (PostgreSQL, Storage, Auth), Google Cloud Run

---

### 🤖 이미지 멀티모달 AI 대화 시스템
**2025.08 - 2025.11** | [HuggingFace](https://huggingface.co/bigdefence)

> 보고 듣고 말하는 AI: 음성·이미지를 동시 이해하여 실시간 음성으로 응답하는 End-to-End 멀티모달 대화 플랫폼

**🎯 핵심 성과**
- ✅ **자체 VLM 개발**: Vision Encoder + LLM 정렬, 2단계 학습 전략(Pre-training / Fine-tuning) 수행
- ✅ **한국어 특화 모델**: Midm-2.0 백본 기반 한국어 VLM 구축 및 HuggingFace 공개
- ✅ **실시간 파이프라인**: Audio/Image → VLM → Streaming TTS 연동, 평균 1.2초 저지연 응답 구현

**🌟 기술 스택**
```
Python, PyTorch, LoRA, DeepSpeed, Gemini API, FastAPI, WebRTC, Whisper, OpenAI TTS
```

---

## 🏆 Awards & Competitions

<div align="center">

| 🗓️ 날짜 | 🏅 대회명 | 🎖️ 순위/결과 |
|:---:|:---|:---:|
| **2025.09** | 잡코리아 AI Challenge - LLM Engineer | **우수상 🥈** |
| **2024.06** | 제1회 해커톤 경진대회 | **최우수상 🥇** |
| **2024.06** | 이스트소프트 파이널 프로젝트 | **우수상 🥈** |
| 2024.05 | Dacon 조류 이미지 분류 AI 경진대회 | 26등 (상위 7%) |

</div>

---

## 🎓 Education & Experience

<table>
<tr>
<td width="50%" valign="top">

### 📖 Education
**이스트소프트 AI 개발자 부트캠프 2기**  
*2024.01 - 2024.06*
- AI/ML 집중 교육 (6개월) 및 프로젝트 기반 학습
- 최우수상·우수상 수상

**한서대학교 무인항공기학과**  
*2024.02 졸업*

</td>
<td width="50%" valign="top">

### 💼 Key Experience
- 🚀 **20+ AI 프로젝트** 개발 및 배포 경험
- 🧠 **LLM 전문성**: VLM, Audio LLM 자체 개발 능력
- 🇰🇷 **한국어 AI 최적화**: 데이터셋 구축 및 모델 튜닝
- 📦 **오픈소스 기여**: HuggingFace 1,500+ 다운로드 달성

</td>
</tr>
</table>

---

## 📞 Contact & Links

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bigdefence)
[![HuggingFace](https://img.shields.io/badge/🤗_HuggingFace-FFD21E?style=for-the-badge)](https://huggingface.co/bigdefence)

### 📧 wjdrkdqls12@gmail.com | 📱 010-3777-8058

---

</div>

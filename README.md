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
- ✅ **문제 해결 능력**: 임베딩 차원 불일치, GPU 메모리 최적화 등 실무 문제 해결

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
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=Flask&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=FastAPI&logoColor=white)
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
**2026.03 - 현재** |

[![Neofish Demo](https://img.youtube.com/vi/qcmQDAeNIpo/maxresdefault.jpg)](https://youtu.be/qcmQDAeNIpo)

> 비정형 시드(뉴스·리포트·내러티브 등)에서 **지식 그래프**를 만들고, **OASIS** 기반 소셜 시뮬레이션으로 집단 행동을 재현한 뒤, **ReportAgent**와 대화·리포트로 해석까지 이어지는 **엔드투엔드 멀티 에이전트 예측 플랫폼**입니다.

**🎯 핵심 기능 및 특장점**
- ✅ **Neo4j 지식 그래프 + 청크 단위 LLM 추출**: 온톨로지 설계 후 문서를 청크로 나누어 엔터티·관계를 추출·적재하고, 시뮬레이션 준비·리포트 도구에 **동일 그래프**를 연결
- ✅ **OASIS(CAMEL-AI) 병렬 시뮬레이션**: Twitter / Reddit / 병렬 모드로 에이전트가 게시·댓글·반응 등 플랫폼 행동을 수행하며, **subprocess**로 웹 API와 장시간 실행을 분리
- ✅ **이중 LLM 전략 (경량·대량 vs 고급 추론)**: 청크 추출·프로필·OASIS 런타임 등 대량 호출과 온톨로지·시뮬 설정 생성·ReportAgent·그래프 도구 연동 분석 등 **추론 집약 구간**에 서로 다른 모델을 매핑해 비용·품질 균형
- ✅ **ReAct 패턴 ReportAgent + GraphTools**: Neo4j 검색·인사이트·에이전트 인터뷰 등 **도구 호출 루프**로 섹션 구조화 리포트 생성 및 **리포트 채팅** 지원
- ✅ **온톨로지 생성 시 Web Grounding(선택)**: Gemini Grounding 연동으로 시드 주제에 맞는 배경 정보를 보강해 **시뮬레이션 맥락**을 정비 (기능 플래그·환경에 따름)
- ✅ **2인 패널 팟캐스트**: Gemini **TTS** 모델로 대화형 오디오 합성, **스크립트**는 경량 LLM + `ThreadPoolExecutor`·레이트 리밋으로 안정적 생성 파이프라인 구성
- ✅ **D3 관계 네트워크 UI**: 노드 검색·줌/팬·이웃 호버 강조·상세 패널로 **그래프 탐색성** 강화 (Vue 3 + D3)

**🔧 기술적 구현 및 시스템 아키텍처**
- **프로세스 분리**: Flask `threaded` API + **subprocess** OASIS 시뮬레이션, 시뮬 디렉터리에 `run_state.json`·액션 로그·**파일 기반 IPC**로 인터뷰 등 비동기 협업
- **회복 탄력성**: LLM·외부 API 호출에 **재시도·백오프** 패턴 적용(서비스 모듈별)
- **Frontend / Backend**: **Vue 3**(Composition API, Vite) · **D3** · **Python Flask** · **OpenAI SDK 호환 LLM** · **Neo4j Bolt** · **OASIS (CAMEL-AI)** · (선택) **Google GenAI** 팟캐스트/그라운딩

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
- ✅ **백테스팅 리스크 매핑**: yfinance 데이터 기반 수익률·MDD 시각화 및 시장 하락 시나리오 정량화 제공

**🔧 기술적 구현 및 시스템 아키텍처**
- **기능 모듈화 (Modularity)**: 유지보수와 기능 확장을 위해 책임을 명확히 분리한 백엔드 구조 최적화 리팩토링
- **AI / Data Pipeline**: Gemini API (Intent & Generation), Tavily (Search), yfinance (Market Data)
- **Frontend / Backend**: React 18, TypeScript, Vite, Supabase / FastAPI, SSE Network Tuning
- **Deployment**: Vercel (Frontend), Docker 컨테이너 배포 (Backend)

---

### 🎨 Magic Canvas: AI 기반 컨텍스트 인식 디자인 에이전트
**2025.11 - 현재** | [Magic Canvas](https://magiccanvas.co.kr/)

[![Magic Canvas Demo](https://img.youtube.com/vi/5pb4txbwxJ8/maxresdefault.jpg)](https://youtu.be/5pb4txbwxJ8)

> 캔버스 위에서 이미지, 텍스트, 화살표, 드로잉을 조합하면 AI가 시각적 의도를 파악하여 고품질 광고 소재(이미지/영상)를 자동 생성하는 **차세대 멀티모달 프롬프트리스 디자인 툴**입니다.

**🎯 핵심 기능 및 특장점**
- ✅ **시각적 의도 해석 (Visual Intent Analysis)**: Gemini 3 Flash를 활용해 캔버스 스냅샷과 사용자 드로잉(화살표, 여백 등)의 문맥을 복합적으로 해석
- ✅ **객체 단위 관계 매핑**: 화면 내 요소들의 공간적 관계와 화살표의 소스-타겟 흐름을 분석하여 가장 이상적인 생성 프롬프트 자동 도출
- ✅ **5대 특화 AI 생성 도구 통합**:
  - **스마트 배경 생성**: 피사체 윤곽, 조명, 톤앤매너에 맞춘 고품질 배경 합성
  - **AI 배경 제거 (누끼)**: 깔끔하고 정밀한 외곽선 제거 기능
  - **광고 배너 팩토리**: 인스타그램, 페이스북, 웹 배너 등 주요 규격에 맞게 텍스트와 레이아웃을 변형하여 일괄 생성
  - **상세페이지 자동 섹션화**: 단일 제품 이미지에서 제품 특징을 파악하여 커머스 상세페이지 기획안 및 섹션 이미지 렌더링
  - **목업 텍스트 리터칭**: OCR 기반으로 이미지 내 기존 텍스트를 파악하고 자연스럽게 지운 뒤 원하는 내용으로 재작성 (Inpainting)
- ✅ **다이내믹 멀티 모델 파이프라인**: 작업 목적에 맞춰 Nano banana, Grok, Kling, Seedream 등 최적의 모델 앙상블 적용
- ✅ **채팅형 UX**: 사이드바 대화창을 통해 에셋 검색, 배경 합성, 캔버스 편집 명령을 자유롭게 주고받는 UX 구현

**🛠️ 기술 스택**
- **Frontend**: React 18, TypeScript, Vite, Fabric.js (Canvas API), Framer Motion, Zustand
- **Backend**: Python 3.12, FastAPI, 비동기 파이프라인(`asyncio`, `run_in_threadpool`), Pillow
- **AI Models**: Gemini 3 Flash/Pro, Grok, Kling, Seedream, OpenAI
- **Infra/Base**: Supabase (PostgreSQL, Storage, Auth), Google Cloud Run (서버리스 배포)

---

### 🤖 이미지 멀티모달 AI 대화 시스템
**2025.08 - 2025.11** | [HuggingFace](https://huggingface.co/bigdefence)

> 보고 듣고 말하는 AI: 음성·이미지를 동시 이해하여 실시간 음성으로 응답하는 End-to-End 멀티모달 대화 플랫폼 구현

**🎯 핵심 성과**
- ✅ **자체 VLM 개발**: 한국어 특화 멀티모달 AI 모델 구축 (HuggingFace 공개)
- ✅ **경량화**: 2B 경량 모델로 엣지/모바일 디바이스에서도 구동 가능

**🔧 기술적 구현**

**1. 자체 VLM 개발 (SmolVLM)**
- **SmolLM2-135M-Instruct + MobileCLIP-B** 기반 경량 Vision-Language Model 직접 개발
- **경량 아키텍처**: 총 0.2B 파라미터로 극도의 경량화 달성 (LLaVA 아키텍처 기반)
- **비전-언어 정렬**: MobileCLIP 비전 특징을 SmolLM2 임베딩 공간으로 매핑

**2. 추가 VLM 개발 (Midm-Vision)**
- **Midm-2.0-Mini-Instruct** 기반 2B 파라미터 한국어 특화 VLM 개발
- Vision Encoder(CLIP) + Vision Projector + LLM 통합 설계

**3. 2단계 학습 전략**
- **Stage 1 (Pre-training)**: Vision Projector만 학습 (비전-언어 정렬)
- **Stage 2 (Fine-tuning)**: Projector + LLM LoRA 공동 미세조정
- **핵심 문제 해결**: Chat Template 마스킹 오류 및 Tokenization Mismatch 해결

**4. LLM-as-a-Judge 평가**
- **Gemini 2.5 Flash Lite 활용**: 의미론적 품질 평가 (정확성, 완전성, 유창성)
- **Flickr8k 평가 결과**: 32%가 70점 이상 (Good/Excellent)

**5. 실시간 멀티모달 파이프라인**
- **Audio + Image → STT → VLM → Streaming TTS → Real-time Voice**
- WebRTC 기반 저지연 스트리밍 (평균 1.2초 응답)

**🌟 기술 스택**
```
Python, PyTorch, SmolLM2, MobileCLIP, LLaVA, LoRA, DeepSpeed, Gemini API, FastAPI, WebRTC, Whisper, OpenAI TTS
```

### 🎙️ BigVox - 한국어 음성 멀티모달 AI 시스템
**2025.03 - 2025.08** | [HuggingFace](https://huggingface.co/bigdefence)

> Speech-to-Speech/Text 통합 시스템: 음성 입력 이해부터 실시간 음성 응답까지 End-to-End 구현

**🎯 핵심 성과**
- ✅ **범용 Speech Projector 설계**: 4개 한국어 LLM 임베딩 차원 불일치 해결, 100% 호환성 확보
- ✅ **실시간 S2S 파이프라인**: Audio → VAD → Speech Encoder → LLM Streaming → CosyVoice2 TTS
- ✅ **Barge-in 구현**: 사용자 끼어들기 감지 시 합성 즉시 중단, 대화 큐 재정렬
- ✅ **모델별 최적화**: 각 LLM의 Chat Template·토크나이저 차이 대응, 맞춤형 전처리

**🔧 지원 LLM 백본**
- LGAI-EXAONE/EXAONE-4.0-1.2B
- HyperCLOVAX-SEED-Text-Instruct-0.5B
- kakaocorp/kanana-1.5-2.1b-instruct-2505
- K-intelligence/Midm-2.0-Mini-Instruct

**🌟 하이라이트**
- Whisper 기반 Mel-spectrogram 변환으로 고급 음성 이해
- 저지연 스트리밍 파이프라인으로 자연스러운 대화 경험
- HuggingFace 오픈소스 공개, 한국어 음성 AI 커뮤니티 기여

### 🏆 잡코리아 AI Challenge - LLM Engineer
**2025.09 - 우수상 🥈** | [GitHub](https://github.com/bigdefence/AI-Challenge-LLM)

> 생성형 AI + RAG로 고품질 채용공고를 자동 생성하는 End-to-End GenAI 파이프라인

**🎯 핵심 성과**
- ✅ **하이브리드 RAG**: FAISS(의미 검색) + BM25(키워드 검색) 앙상블로 검색 정확도 대폭 향상
- ✅ **Docling PDF 추출**: 레이아웃·표까지 정밀 파싱, 텍스트 품질 향상
- ✅ **안전성 가드레일**: 민감·차별 표현 자동 탐지·교정, 안전한 채용공고 생성 보장
- ✅ **성능 최적화**: 임베딩 배치 인코딩 + TTL 캐시, 응답 시간 단축

**🔧 기술 스택**
- FastAPI, FAISS, BM25, Docling, LiteLLM, gpt-4o-mini

---

### 📄 ReportCast - 실시간 AI 검색 기반 보고서 & 팟캐스트 생성
**2025.01 - 2025.02** | [GitHub](https://github.com/bigdefence/ReportCast)

> Gemini Grounding + 멀티모달 AI로 보고서·팟캐스트 자동 생성

**🎯 핵심 기능**
- **실시간 AI 검색**: Gemini Grounding, Flash(빠른 응답) + Thinking(심층 분석) 듀얼 모델
- **보고서 생성**: 서론-본론-결론 구조화, Imagen3 표지 디자인, ReportLab PDF 변환
- **팟캐스트 생성**: ChatGPT 대본 작성, OpenAI TTS 음성 합성(Onyx·Nova), 배경음악 믹싱

---

### 🎨 OmniVerse - 멀티모달 AI 통합 플랫폼
**2024.07 - 2024.08** | [GitHub](https://github.com/bigdefence/OmniVerse)

> Gemini 챗봇, 얼굴 분석, 이미지 분석, AI 패션 스타일리스트 All-in-One

**🎯 핵심 기능**
- **Gemini 챗봇**: 대화형 인터페이스로 다양한 질문 응답
- **얼굴 분석**: MediaPipe 감지 + Swin Transformer 직접 구현으로 외모 점수 측정
- **이미지 분석**: Gemini 비전 모델로 객체·배경·분위기·색상 상세 분석
- **AI 패션 스타일리스트**: FLUX/Stable Diffusion으로 맞춤형 패션 이미지 생성

---

### 💭 기억나래 - AI 기억 보조 시스템
**2024.06** | [GitHub](https://github.com/bigdefence/hackathon)

> 고령자·치매 환자를 위한 음성 대화 + 감성 일기 + 그림일기 자동 생성

**🎯 핵심 기능**
- **음성 대화**: STT/TTS 기반 자연스러운 음성 인터페이스
- **AI 감성 일기**: ChatGPT로 대화 내용을 감정 담긴 일기로 자동 변환
- **그림일기 생성**: DALL-E 3로 수채화 스타일 이미지 자동 생성
- **보호자 모니터링**: 활동 추적, 감정 변화 시각화, 비정상 패턴 알림

---

### 🎵 MusicFace - AI 얼굴 분석 기반 맞춤형 음악 생성
**2024.05 - 2024.06** | [GitHub](https://github.com/bigdefence/Music-Face)

> 얼굴 분석으로 표정·나이·성별 파악 → LLM 음악 추천 → SUNO AI 생성

**🎯 핵심 기능**
- **얼굴 검출**: MediaPipe로 얼굴 영역 검출 및 전처리
- **Vision Transformer**: BEiT-V2(표정 인식) + Swin-V2(나이·성별 판별)
- **음악 추천**: LLaMA-3로 얼굴 특성 → 장르·분위기·템포 매핑
- **음악 생성**: SUNO AI로 맞춤형 음악 자동 생성 (30초~3분)

---

### 📚 Additional Projects

<details>
<summary><b>🔍 AI Search & RAG Systems</b> (클릭하여 펼치기)</summary>

#### AI-Powered Search & Content Generation Platform (2024.08 - 2024.11)
- Google, Naver, YouTube API 통합 검색 + asyncio 비동기 처리
- RAG(FAISS + BM25 앙상블)로 사용자 쿼리 관련 콘텐츠 검색
- ChatGPT/Gemini로 검색 결과 분석·요약 및 심층 질문 응답
- Flask 웹 인터페이스 + GCP 배포
- [GitHub: SearchCast](https://github.com/bigdefence/SearchCast) | [GitHub: AI Search Engine](https://github.com/bigdefence/search)

#### 난독화된 한글 리뷰 데이터 복원 (2025.01 - 2025.02)
- 철자 오류·띄어쓰기 왜곡 텍스트 전처리 및 LLM 문맥 기반 복원
- QLoRA(Unsloth) 파인튜닝: 학습시간 2배 단축, 메모리 50% 절감
- [GitHub](https://github.com/bigdefence/Restoration-of-obfuscated-Korean)

</details>

<details>
<summary><b>🧠 LLM Development & Fine-tuning</b> (클릭하여 펼치기)</summary>

#### Bigdefence LLM 아키텍처 설계 및 사전학습 (from scratch)
- Transformer 기반 한국어 최적화 모델 설계·사전학습
- LLaMA 아키텍처 분석, GQA, RoPE 등 최신 기법 적용
- 원시 텍스트 수집부터 전처리, 토크나이징, 학습, 추론까지 전 과정 구현
- [GitHub](https://github.com/bigdefence/LLM-study)

#### LLM Fine-Tuning RAG 챗봇 (2024.05 - 2024.07)
- RAG 시스템 (FAISS, SentenceTransformer) + QLoRA Fine-tuning
- Unsloth로 학습시간 2배 단축, 메모리 55% 절감
- HuggingFace 모델 배포 (1,200+ 다운로드)
- [GitHub](https://github.com/bigdefence/rag_chatbot)

#### 음성지원 챗봇 (2024.06 - 2024.07)
- Whisper STT + LLaMA-3-Korean + gTTS 음성 출력
- FastAPI REST API 구현
- [GitHub](https://github.com/bigdefence/stt-tts-chatbot)

</details>

<details>
<summary><b>👤 Computer Vision & Face Analysis</b> (클릭하여 펼치기)</summary>

#### 나의 외모점수는? (2023.10 - 2023.11)
- MediaPipe 얼굴 검출 + Vision Transformer(Swin-V2) 구현
- Streamlit 웹 인터페이스, EDA 수행
- [Live Demo](https://facescore.streamlit.app) | [GitHub](https://github.com/bigdefence/face_score)

#### Facefy (2024.08)
- Google Gemini AI 얼굴 분석 + 관상학적 해석·운세 예측
- Flask 웹 인터페이스 + GCP 배포
- [GitHub](https://github.com/bigdefence/facefy)

</details>

---

## 🏆 Awards & Competitions

<div align="center">

| 🗓️ 날짜 | 🏅 대회명 | 🎖️ 순위/결과 |
|:---:|:---|:---:|
| **2025.09** | 잡코리아 AI Challenge - LLM Engineer | **우수상 🥈** |
| **2024.06** | 제1회 해커톤 경진대회 | **최우수상 🥇** |
| **2024.06** | 이스트소프트 파이널 프로젝트 | **우수상 🥈** |
| 2024.05 | Dacon 조류 이미지 분류 AI 경진대회 | 26등 (상위 7%) |
| 2024.04 | Dacon 모델 튜닝 챌린지 | 16등 (상위 5%) |
| 2024.03 | 웹 로그 기반 조회수 예측 해커톤 | 26등 (상위 10%) |

</div>

---

## 🎓 Education & Experience

<table>
<tr>
<td width="50%" valign="top">

### 📖 Education
**이스트소프트 AI 개발자 부트캠프 2기**  
*2024.01 - 2024.06*
- AI/ML 집중 교육 (6개월)
- 프로젝트 기반 학습
- 최우수상·우수상 수상

**한서대학교 무인항공기학과**  
*2024.02 졸업*

</td>
<td width="50%" valign="top">

### 💼 Key Experience
- 🚀 **20+ AI 프로젝트** 개발·배포
- 🧠 **LLM 전문**: VLM, Audio LLM 개발
- 🇰🇷 **한국어 AI**: 데이터셋 구축·모델 개발
- 📦 **오픈소스**: HuggingFace 1,500+ 다운로드
- 🏆 **수상**: 최우수상 🥇, 우수상 🥈 × 2

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

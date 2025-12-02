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
| **💡 프로젝트** | 20+ AI 프로젝트 개발·배포 |
| **🔬 모델 개발** | VLM·Audio LLM 자체 개발 |

</div>

---

## 🏆 Featured Projects

### 🎨 AI Ad Maker – Magic Canvas Agent
**2025.12** | 

> 드래그 앤 드롭으로 이미지를 배치하고, 화살표/텍스트로 의도를 그려 넣으면 Gemini가 자연스럽고 일관성 있는 합성 컷을 생성하는 프롬프트리스 Magic Canvas 툴

**🎯 핵심 가치**
- ✅ **객체 단위 추출**: 선택 영역 안의 이미지·화살표·텍스트·프리드로잉을 별도 객체로 분리
- ✅ **관계 해석 엔진**: 화살표 시작/끝 좌표를 기반으로 “소스 → 타겟” 매핑 (예: 모자 → 인물)
- ✅ **Gemini 멀티 이미지 입력**: 분리된 모든 이미지를 `types.Part.from_bytes()`로 변환하여 Gemini 2.5 Flash Image에 동시에 전달
- ✅ **일관성 보존 프롬프트**: 얼굴/로고/재질/조명을 그대로 유지하도록 자동 지시
- ✅ **경량 UI**: 캔버스 집중형 워크플로

**🔧 시스템 개요**
```
React + Fabric.js Canvas  ── 객체 리스트(JSON) ──▶ FastAPI 서버 ──▶ Gemini 2.5 Flash Image
          ▲                         │                               │
          └──────── 생성 결과 (base64) ◀──────────────────────────────┘
```
1. 사용자가 캔버스에 이미지·화살표·텍스트를 배치하고 영역을 선택
2. 프론트엔드가 영역 내 객체를 추출하여 서버에 전달
3. 서버는 화살표 관계를 분석해 “소스 → 타겟” 명령을 프롬프트에 포함
4. Gemini에 멀티 이미지 입력으로 합성 요청 후 결과를 다시 캔버스에 배치

**🧩 API 하이라이트**
- `POST /api/generate`: 전체 캔버스 캡처 기반 빠른 합성 (폴백)
- `POST /api/generate-from-objects`: 이미지·화살표·텍스트 객체 기반 고품질 합성 (권장)

**🛠️ 기술 스택**
```
Frontend  : React 18, TypeScript, Vite, Fabric.js, Axios
Backend   : Python 3.12, FastAPI, Pillow, Gemini
AI Models : Gemini 2.5 Flash Image (멀티 이미지 입력, 고일관성 프롬프트)
```

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

<sub>⭐ 더 나은 AI로 세상과 소통하는 개발자, 정강빈입니다. ⭐</sub>

</div> 

# 정강빈 (Kangbin Jeong)
### ML/DL Developer | AI Engineer
![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=bigdefence)

## 🚀 About Me
코드로 세상을 바꾸는 개발자를 꿈꾸고 있습니다. 차별화된 서비스를 만들어내며, 사람들이 필요로 하는 것이 무엇인지 고민하는 AI 개발자입니다.

## 🛠 Tech Stack
### Languages & Frameworks
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=PyTorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=TensorFlow&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=Flask&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=OpenCV&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=Streamlit&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

### Tools & Platforms
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=google-cloud&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)

https://github.com/user-attachments/assets/75e7a99e-df4a-4e28-876f-cf736503f9bf



https://github.com/user-attachments/assets/c1bbae8f-61cf-4605-86bc-7fe767136010


https://github.com/user-attachments/assets/cfaba4f3-3886-4152-ac54-42af4ea0e84b


## 🏆 Projects

### 🎙️ BigVox 한국어 음성 멀티모달 시스템 개발 (2025.06 ~ 진행중)
"음성으로 소통하는 AI: 음성 입력을 이해하고 지능적으로 응답하는 멀티모달 LLM 시스템 구현"<br>
BigVox는 최신 딥러닝 기술을 활용한 고성능 음성 입력 기반 멀티모달 AI 모델입니다. 음성 명령을 이해하고 적절한 텍스트 응답을 생성하는 기능을 제공하며, **허깅페이스에 오픈소스로 공개**되어 누구나 자유롭게 사용할 수 있습니다.

- **End-to-End 음성 명령 이해 시스템**: 원시 오디오 입력부터 지능적인 텍스트 응답까지 완전한 파이프라인 구현
- **멀티모달 아키텍처**: Audio → Speech Encoder → Speech Projector → LLM Backbone → Text Response
- **다중 언어 모델 백본 지원**: 
  - **Llama-3.2-1B-Instruct**: Meta의 최신 경량화 언어 모델을 활용한 효율적인 명령 이해 및 응답 생성
  - **HyperCLOVAX-SEED-Text-Instruct-0.5B**: 네이버의 한국어 특화 모델로 한국어 음성 명령 이해 및 응답 품질 극대화
- **고급 음성 이해**: Whisper 기반 Mel-spectrogram 변환으로 음성 명령의 의미와 맥락을 정확히 파악
- **지능형 명령 처리**: 음성 입력을 LLM이 이해할 수 있는 형태로 변환하여 적절한 instruction following 수행
- **모델 적응형 추론**: 언어 모델별 최적화된 토크나이저 및 생성 매개변수로 각 모델의 성능 최대화


### 🎙️ Speech-To-Speech 한국어 음성 멀티모달 개발 (2025.03 ~ 2025.06)
"영어 중심 한계를 넘어: 한국어 전용 Speech-to-Speech 멀티모달 시스템 End-to-End 개발"

- **End-to-End 음성 대화 시스템**: 음성 입력부터 음성 출력까지 완전한 파이프라인 구현
- **멀티모달 아키텍처**: Audio → Speech Encoder → Downsampling Adaptor → LLM Backbone → Speech Projector → Speech Decoder → Audio
- **한국어 특화 학습**: 직접 구축한 한국어 음성 데이터셋으로 2단계 학습 과정 수행
  - Stage 1: 음성 쿼리와 텍스트 응답을 활용해 음성 인코더와 LLM의 embedding 공간을 정렬하며, LLM에 LoRA로 멀티모달 적응을 수행
  - Stage 2: 음성 쿼리-음성 토큰 기반으로 speech projector 및 decoder를 고정된 LLM 위에 학습시켜, 실제 음성 생성 능력을 부여
- **고성능 최적화**: PyTorch, Transformers, DeepSpeed, LoRA/PEFT 활용한 효율적 학습
- **TTS 통합**: CosyVoice, Matcha-TTS를 활용한 자연스러운 음성 합성


### Bigdefence LLM 아키텍처 설계 및 사전학습(LLaMA 기반)
Transformer 아키텍처를 기반으로 한국어에 최적화된 모델을 설계하고 사전학습했습니다. LLaMA 모델의 핵심 아키텍처를 분석하여 자체 모델인 'Bigdefence LLM'을 구축했습니다.
- LLaMA의 핵심 구조를 분석하고 Grouped Query Attention(GQA), Rotary Position Embedding(RoPE) 등 최신 기법을 적용하여 효율적인 모델 구조 구현
- LLaMA 모델을 기반으로 Bigdefence(정강빈) 모델 구축
- 원시 텍스트 수집부터 전처리, 토크나이징, 모델 학습, 추론까지 언어 모델 개발 파이프라인 설계 및 구현
- 향후 계획:
   - 다양한 한국어 도메인 데이터셋 추가를 통해 언어 이해력 확장
   - SFT(Supervised Fine-Tuning) 기법 적용으로 Instruction 기능 향상 
- [GitHub Repository](https://github.com/bigdefence/LLM-study)

### ReportCast (2025.01 ~ 2025.02)
실시간 인공지능 검색으로 팟캐스트 및 보고서 생성 애플리케이션
- Gemini Grounding API로 최신 웹 검색 결과 수집 후 콘텐츠 생성
- 서론·본론·결론 구조의 자동 보고서 생성 및 심층 분석 적용
- Gemini-2.0-flash/-thinking 모델로 빠른 응답시간과 정교한 답변 제공
- Imagen3로 보고서 표지 자동 디자인, ReportLab + NanumGothic 폰트로 PDF 변환
- ChatGPT API로 팟캐스트 대본 자동 작성, OpenAI TTS API로 음성(.mp3) 변환·믹싱
- Flask 기반 웹 인터페이스로 사용자 친화적 서비스 제공  
- [GitHub Repository](https://github.com/bigdefence/ReportCast)
  
### 난독화된 한글 리뷰 데이터 복원 (2025.01 ~ 2025.02)
난독화된 텍스트 자동 복원 시스템 개발
- 철자 오류·띄어쓰기 왜곡 등 난독화된 리뷰 텍스트 전처리
- ChatGPT·Gemini·LLaMA·EXAONE·Gemma 등 LLM으로 문맥 기반 복원
- QLoRA(Unsloth) 활용 파인튜닝: 학습시간 2배 단축, 메모리 50% 절감
- 자주 발생하는 오류 패턴 사전 정의 후 복원 알고리즘에 반영
- [GitHub Repository](https://github.com/bigdefence/Restoration-of-obfuscated-Korean)

### SearchCast (2024.10 - 2024.11)
실시간 AI 기반 팟캐스트 생성 플랫폼
- 실시간 AI 검색엔진 연계 및 데이터 수집
- RAG(BM25, FAISS 앙상블) 이용하여 사용자 쿼리와 관련된 콘텐츠의 검색 구현
- ChatGPT API를 활용하여 팟캐스트 대본 자동 생성, 사용자 입력 기반 맞춤형 스크립트 제공
- OpenAI TTS API를 활용하여 대본을 음성 파일(.mp3)로 변환, 자연스러운 음성 생성
- 배경음악 추가 및 팟캐스트 믹싱
- Flask 기반 웹 인터페이스
- [GitHub Repository](https://github.com/bigdefence/SearchCast)

### AI Search Engine (2024.08 - 2024.09)
통합 검색엔진 시스템
- Google, Naver, YouTube API 통합 검색
- asyncio/aiohttp 활용 비동기 처리
- RAG(BM25, FAISS 앙상블) 이용하여 사용자 쿼리와 관련된 콘텐츠의 검색 구현
- ChatGPT와 Gemini 모델을 사용하여 검색 결과를 바탕으로 심층적인 질문 응답을 생성하고, 검색 결과를 분석하고 요약
- Flask 기반 웹 인터페이스
- GCP 기반 웹 애플리케이션 배포
- [GitHub Repository](https://github.com/bigdefence/search)

### Facefy (2024.08)
AI 기반 얼굴 분석 서비스
- Google Gemini AI 활용 얼굴 분석
- 관상학적 해석 및 운세 예측
- 궁합 분석 기능 구현
- Flask 기반 웹 인터페이스
- GCP 활용 웹 애플리케이션 배포
- [GitHub Repository](https://github.com/bigdefence/facefy)

### OmniVerse (2024.07 - 2024.08)
멀티모달 한국어 챗봇
- Google Gemini 모델 기반 대화형 인터페이스
- MediaPipe 활용 얼굴 감지 및 분석
- 나의 외모점수는?
   - 외모점수 Vision Transformer 구현(Swin Transformer)
- AI 패션 스타일리스트 기능
   - 사용자의 특징(성별, 나이대, 체형 등)을 고려한 맞춤형 스타일 제안
   - Text-to-Image(FLUX, Stable Diffusion) 추천된 패션 스타일 이미지 생성
- [GitHub Repository](https://github.com/bigdefence/OmniVerse)

### 음성지원 챗봇 (2024.06 - 2024.07)
LLM 기반 음성 지원 챗봇
- Whisper 모델 활용 음성 인식
- LLaMA-3-Korean 모델 기반 대화 응답 생성
- gTTS Text-to-Speech 음성 출력
- FastAPI 기반 REST API 구현
- [GitHub Repository](https://github.com/bigdefence/stt-tts-chatbot)

### LLM Fine-Tunning RAG 챗봇 (2024.05 - 2024.07)
개인화된 LLM 개발 및 RAG 시스템
- RAG 시스템 구현 (FAISS, SentenceTransformer)
- QLoRA 기반 모델 Fine-tuning
  - Unsloth를 이용하여 학습 시간 및 메모리 효율 향상(학습시간 약 2배 단축, 메모리 사용량 약 55% 절감) 
- HuggingFace 모델 배포 (1200+ 누적 다운로드 달성)
- [GitHub Repository](https://github.com/bigdefence/rag_chatbot)

### 기억나래 (2024.06)
외로운 일상의 소중한 기억을 지켜주는 인공지능 '기억나래'
- STT/TTS 기술 활용 자연스러운 음성 대화
- ChatGPT API 활용 대화 및 일기 생성
- DALL-E 3 모델 활용 그림일기 생성
- 보호자용 모니터링 대시보드 구현
- [GitHub Repository](https://github.com/bigdefence/hackathon)

### MusicFace (2024.05 - 2024.06)
얼굴 분석을 통한 '나만의 음악' 생성 인공지능 'Music Face'
- MediaPipe 활용 얼굴 검출
- Vision Transformer(BEiT-V2, Swin-V2)모델 구현
- 얼굴 분석 내용 기반 LLaMA3를 활용하여 음악 장르 및 분위기 추천 시스템 구현
- LLaMA-3 프롬프트 엔지니어링 수행
- LLaMA-3 활용 음악 장르 추천
- 음악 생성 및 다운로드 시스템 구현
- Gradio 웹 인터페이스 
- [GitHub Repository](https://github.com/bigdefence/Music-Face)

### 나의 외모점수는? (2023.10 - 2023.11)
AI 기반 외모 점수 측정 서비스
- 데이터셋 분석 및 전처리를 위한 EDA 수행
- MediaPipe 활용 얼굴 검출
- Vision Transformer(Swin-V2) 모델 구현
- Streamlit 기반 웹 인터페이스
- [Live Demo](https://facescore.streamlit.app)
- [GitHub Repository](https://github.com/bigdefence/face_score)

## 🏆 Awards & Recognition

| 연도 | 수상 내역 | 순위 |
|------|-----------|------|
| 2024.06 | 제1회 해커톤 경진대회 | **최우수상** 🥇 |
| 2024.06 | 이스트소프트 파이널 프로젝트 | **우수상** 🥈 |
| 2024.05 | Dacon 조류 이미지 분류 AI 경진대회 | **26등 (상위 7%)** |
| 2024.04 | Dacon 모델 튜닝 챌린지 | **16등 (상위 5%)** |
| 2024.03 | 웹 로그 기반 조회수 예측 해커톤 | **26등 (상위 10%)** |

---

## 📚 Education & Experience

**🎓 Education**
- **이스트소프트 AI 개발자 부트캠프 2기** (2024.01 - 2024.06)
- **한서대학교 무인항공기학과** (2024.02 졸업)

**💼 Key Experience**
- **20+ AI 프로젝트** 개발 및 배포 경험
- **LLM** 전문 분야 
- **한국어 AI** 데이터셋 구축 및 모델 개발
- **오픈소스 기여**: HuggingFace 모델 1,200+ 다운로드

---

## 🔗 Connect with Me
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/bigdefence)
[![Notion](https://img.shields.io/badge/Notion-000000?style=flat-square&logo=notion&logoColor=white)](https://navy-ellipse-684.notion.site/afcd3d1da3b743e4bef129aa7a5150ae?pvs=74)
[![HuggingFace](https://img.shields.io/badge/HuggingFace-FF9D00?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co/bigdefence)

## 📧 Contact
- Email: wjdrkdqls12@gmail.com
- Phone: 010-3777-8058 

# 정강빈 (Kangbin Jeong)
### ML/DL Developer | AI Engineer
![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=bigdefence)

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fbigdefence&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)

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

### Tools & Platforms
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=google-cloud&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)

## 🏆 Projects






https://github.com/user-attachments/assets/a1360476-396d-4e04-a741-796aa17bda9c





https://github.com/user-attachments/assets/55bc31d8-ab36-4c8a-a280-73f128005da5





https://github.com/user-attachments/assets/cfaba4f3-3886-4152-ac54-42af4ea0e84b




![스크린샷 2025-01-26 112129](https://github.com/user-attachments/assets/432794e2-f023-45d5-a12b-0e6d00e45807)

### KMMLU(Criminal-Law) Evaluation Agent (2025.02)
Criminal-Law 분야의 법률 질문에 대해 OpenAI API와 FAISS 기반 검색 시스템을 활용하여 질문-응답 평가를 수행
- PyPDF2를 사용하여 PDF 파일에서 텍스트를 추출하고, 불필요한 공백 및 특수문자 제거
- OpenAI의 text-embedding-3-small를 통해 각 청크에 대한 임베딩 벡터 생성
- 주어진 질문에 대해 관련 chunk를 검색하여, 답변 생성에 참고할 문맥(context) 제공
- 검색된 문맥과 함께 형사법 관련 문제의 선택형 질문(옵션 A~D)에 대한 프롬프트 생성
- OpenAI Batch API를 호출하여 모델 응답을 받고, 실제 정답과 비교하여 평가 정확도 산출
- 이전에 계산된 임베딩 결과는 캐시 파일(.pkl)로 저장하여, 반복 실행 시 재계산 방지
- Docker를 사용함으로써, 의존성 관리 및 환경 설정이 용이하며, 동일한 환경에서 일관된 실행 결과 보장
- [GitHub Repository](https://github.com/bigdefence/kmmlu)
### ReportCast (2025.01 ~ 2025.02)
실시간 인공지능 검색으로 팟캐스트 및 보고서 생성 애플리케이션
- Gemini Grounding API를 활용하여 최신 검색 결과를 기반으로 콘텐츠 생성 및 팟캐스트·보고서 제작
- Gemini API를 활용하여 서론-본론-결론 구조의 자동 보고서 생성 및 심층 분석 내용 포함
- ReportLab을 이용하여 PDF 변환, 한글 폰트(NanumGothic) 적용으로 가독성 향상
- ChatGPT API를 활용하여 팟캐스트 대본 자동 생성, 사용자 입력 기반 맞춤형 스크립트 제공
- OpenAI TTS API를 활용하여 대본을 음성 파일(.mp3)로 변환, 자연스러운 음성 생성
- 배경음악 추가 및 팟캐스트 믹싱
- Flask 기반 웹 인터페이스
- [GitHub Repository](https://github.com/bigdefence/ReportCast)
  
### 난독화된 한글 리뷰 데이터 복원 (2025.01 ~ 진행중)
난독화된 텍스트 자동 복원 시스템 개발
- 난독화된 한국어 텍스트(철자 오류, 띄어쓰기 왜곡 등) 복원
- LLM(ChatGPT, Gemini, LLaMA, EXAONE, Gemma)를 활용해 문맥 기반 복원 수행
- 자주 발생하는 한국어 오류 유형(모음/자음 대치, 오타, 문장 구조 왜곡)을 분석하여 복원 규칙 정의
- LLaMA, EXAONE, GEMMA 등 오픈소스 모델을 특정 도메인(예: 난독화된 리뷰 데이터)에 맞춰 파인튜닝
- 데이터 전처리부터 모델 학습 구현
- Unsloth(QLoRA)를 이용하여 학습 시간 및 메모리 효율 향상(학습시간 약 2배 단축, 메모리 사용량 약 50% 절감)
- 잘못된 자음/모음, 불완전한 단어, 띄어쓰기 오류를 분석해 복원 알고리즘에 적용
- 복잡한 문장 구조에서도 문맥 정보를 기반으로 문법적으로 올바른 문장 생성
- 빈도가 높은 난독화 패턴을 사전 정의하고, 이를 복원 프로세스에 반영
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
외로운 일상의 소중한 기억을 지켜주는 인공지능 ‘기억나래’
- STT/TTS 기술 활용 자연스러운 음성 대화
- ChatGPT API 활용 대화 및 일기 생성
- DALL-E 3 모델 활용 그림일기 생성
- 보호자용 모니터링 대시보드 구현
- [GitHub Repository](https://github.com/bigdefence/hackathon)

### MusicFace (2024.05 - 2024.06)
얼굴 분석을 통한 ‘나만의 음악’ 생성 인공지능 ‘Music Face’
- MediaPipe 활용 얼굴 검출
- Vision Transformer(BEiT-V2, Swin-V2)모델 구현
- 얼굴 분석 내용 기반 LLaMA3를 활용하여 음악 장르 및 분위기 추천 시스템 구현
- LLaMA-3 프롬프트 엔지니어링 수행
- LLaMA-3 활용 음악 장르 추천
- 음악 생성 및 다운로드 시스템 구현
- Gradio 웹 인터페이스 
- [GitHub Repository](https://github.com/bigdefence/Music-Face)

### 나의 MBTI는? (2023.11 - 2023.12)
외모 기반 MBTI 예측 서비스
- MBTI 데이터셋 크롤링
- MediaPipe 활용 얼굴 검출
- EfficientNet 모델 구현
- MBTI에 대한 성격, 연애 스타일, 직업, 유명인 소개 구현
- Streamlit 기반 웹 인터페이스
- [Live Demo](https://facembti.streamlit.app)
- [GitHub Repository](https://github.com/bigdefence/mbti)

### 나의 외모점수는? (2023.10 - 2023.11)
AI 기반 외모 점수 측정 서비스
- 데이터셋 분석 및 전처리를 위한 EDA 수행
- MediaPipe 활용 얼굴 검출
- Vision Transformer(Swin-V2) 모델 구현
- Streamlit 기반 웹 인터페이스
- [Live Demo](https://facescore.streamlit.app)
- [GitHub Repository](https://github.com/bigdefence/face_score)

### 해양 익수자 수색 QuadPlane (2023.09 - 2023.11)
드론 기반 해양 익수자 수색 시스템
- YOLOv8 활용 인물 검출
- MjpgStreamer 활용 실시간 영상 전송
- 라즈베리파이 기반 제어 시스템 구축
- GCS 영상 처리 시스템 개발

### 해양 구조 다목적 드론 (2023.09 - 2023.11)
해양 구조용 드론 시스템
- YOLOv8 활용 인물 검출
- MjpgStreamer 활용 실시간 영상 전송
- 라즈베리파이 기반 제어 시스템 구축
- GCS 영상 처리 시스템 개발

## 🏅 Awards & Achievements
- 제1회 해커톤 경진대회 최우수상 (2024.06)
- 이스트소프트 파이널 프로젝트 우수상 (2024.06)
- Dacon 조저해상도 조류 이미지 분류 AI 경진대회 26등, 상위 7% (2024.05)
- Dacon 모델 튜닝 챌린지: 월간 데이콘 파일럿 16등, 상위 5% (2024.04)
- 웹 로그 기반 조회수 예측 해커톤 26등, 상위 10% (2024.03)
- UCC 공모전 최우수상 (2023.12)
- Startup 경진대회 우수상 (2023.11)
- 캡스톤 경진대회 우수상 (2023.11)

## 📚 Education
- AI 개발자 2기 부트캠프 - 이스트소프트 (2024.01 - 2024.06)
- 한서대학교 무인항공기학과 (2024.02 졸업)

## 🔗 Connect with Me
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/bigdefence)
[![Notion](https://img.shields.io/badge/Notion-000000?style=flat-square&logo=notion&logoColor=white)](https://navy-ellipse-684.notion.site/afcd3d1da3b743e4bef129aa7a5150ae?pvs=74)
[![HuggingFace](https://img.shields.io/badge/HuggingFace-FF9D00?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co/bigdefence)

## 📧 Contact
- Email: wjdrkdqls12@gmail.com
- Phone: 010-3777-8058


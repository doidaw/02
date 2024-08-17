# 👩‍❤️‍👨 AI-based Affection Scoring Chatbot

**Generative AI Development Project, Naver HyperCLOVA x LangChain Korea**  
*5th Place - July 2024*

## 🤖 Overview

Welcome to the repository of the AI-based Affection Scoring Chatbot. Developed by the KUBIG team from Korea University, consisting of Bae Ji-won, Sim Seung-hyun, Jeong Ha-yeon, and Jeong Hae-won. This project focuses on evaluating real-time affection scores in romantic and daily conversations. Utilizing HyperCLOVA and LangChain, we have developed a chatbot that specializes in analyzing Korean sentiment expressions.

---

## Features 

### 💬 Real-time Affection Scoring

- **Target Users**: Individuals in romantic and daily conversations in their 20s
- **Components**: Real-time sentiment analysis and affection score computation
- **Customization**: Provides real-time affection scores based on user conversations

### 📊 Data and Model

- **Model**: Fine-tuned KcELECTRA model with the KOTE dataset to label emotions, with each label assigned an affection score.
- **Scoring Method**:
  1. **Affection Score per Turn**: The affection metric is calculated as the product of the probability of each emotion label and the weight of the emotion score.
  2. **Contextual Understanding**: The overall affection score considers the entire conversation context by summing the product of emotion label probabilities and weights, with more recent turns receiving greater weight (current turn number/total conversation turns).
- **KoBERT Word Embeddings**: Used to calculate the cosine similarity between emotion labels like ‘Excitement’, ‘Interest’, ‘Affection’, and ‘Love’ to derive scores.

### 🌐 Web Application

- **Tech Stack**: Web application built with Streamlit
- **User Interface**: Interactive chatbot providing real-time feedback on conversations

---

## Project Structure

### 1. User Information Input
- **Basic Info**: Name, gender, age

### 2. Conversation Analysis and Affection Scoring
- **Sentiment Analysis**: Extracts emotion labels for each utterance
- **Affection Scoring**: Calculates affection scores using cosine similarity with emotion labels

### 3. Web Application Implementation
- **Streamlit**: Provides a real-time chat interface between users and the chatbot
- **Affection Score**: Displays cumulative affection scores at the end of conversations

---

## Limitations and Future Work

1. **Complexity of Affection Scoring**: Challenges in accurately calculating real-time affection scores
2. **Data Limitations**: Constraints of the Korean sentiment dataset
3. **Improvement Areas**:
   - Enhancing the natural flow of conversations
   - Increasing the accuracy of sentiment analysis models
   - Improving UI/UX

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- KUBIG team members from Korea University
- Support from NAVER Cloud and LangChain Korea

---

# 👩‍❤️‍👨 AI 기반 호감도 평가 챗봇

**Generative AI Development Project, Naver HyperCLOVA x LangChain Korea**  
*5위 - 2024년 7월*

## 🤖 개요

AI 기반 호감도 평가 챗봇 리포지토리에 오신 것을 환영합니다. 이 프로젝트는 고려대학교 데이터 사이언스 & 인공지능 학회 KUBIG 팀에 의해 개발되었으며, 팀원은 배지원, 심승현, 정하연, 정해원입니다. 이 챗봇은 연애 및 일상 대화에서 실시간으로 호감도를 평가하는 기능을 제공합니다. HyperCLOVA와 LangChain을 활용하여 한국어 감정 표현에 초점을 맞춘 챗봇을 개발하였습니다.

---

## 기능

### 💬 실시간 호감도 평가

- **대상 사용자**: 연애 관계와 일상 대화를 나누는 20대
- **구성 요소**: 실시간 감정 분석 및 호감도 점수 계산
- **커스터마이징**: 사용자의 대화에 따라 실시간으로 호감도 점수 제공

### 📊 데이터 및 모델

- **모델**: KcELECTRA 모델을 KOTE 데이터셋으로 파인 튜닝하여 감정 레이블을 달고, 각 감정 레이블마다 설렘 점수를 부여함.
- **점수 산출 방식**:
  1. **각 대화 턴마다 호감도 점수 산출**: 호감도 메트릭은 AI의 답변 문장에 대한 감정 레이블 각각의 확률과 감정 점수별 가중치를 곱하여 계산됨.
  2. **맥락을 고려한 대화 전반적 분위기 파악**: AI의 답변 문장에 대한 감정 레이블의 확률과 감정 점수별 가중치를 모두 더한 후, 최신 턴에 더 큰 가중치를 부여하여 전체 대화의 분위기를 종합적으로 파악함.
- **KoBERT 워드 임베딩**: ‘설렘’, ‘관심’, ‘호감’, ‘사랑’과 같은 감정 라벨 간의 코사인 유사도 점수의 평균을 활용하여 점수화함.

### 🌐 웹 애플리케이션

- **기술 스택**: Streamlit을 사용한 웹 애플리케이션
- **사용자 인터페이스**: 사용자와 챗봇 간의 상호작용을 통해 실시간 피드백 제공

---

## 프로젝트 구조

### 1. 사용자 정보 입력
- **기본 정보**: 이름, 성별, 나이

### 2. 대화 분석 및 호감도 계산
- **감정 분석**: 각 발화에 대해 감정 레이블 도출
- **호감도 계산**: 감정 레이블과 코사인 유사도를 활용한 호감도 점수 계산

### 3. 웹 애플리케이션 구현
- **Streamlit**: 사용자와 챗봇 간의 실시간 대화 인터페이스 제공
- **호감도 점수**: 대화 종료 시 누적 호감도 점수 표시

---

## 한계점 및 향후 작업

1. **호감도 계산의 복잡성**: 실시간으로 정확한 호감도 계산의 어려움
2. **데이터 제한**: 한국어 감정 데이터셋의 제한
3. **개선 사항**:
   - 대화 흐름의 자연스러움 향상
   - 감정 분석 모델의 정확도 증가
   - UI/UX 개선

---

## 라이센스

이 프로젝트는 MIT 라이센스 하에 라이센스됩니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.

---

## 감사 인사

- 고려대학교 데이터 사이언스 & 인공지능 학회 KUBIG 팀원들
- NAVER Cloud와 LangChain Korea의 지원

---

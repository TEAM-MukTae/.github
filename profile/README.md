
<div align="center">
  
  ![image](https://github.com/user-attachments/assets/48733702-6e7b-4bdc-bd9f-780443ebc734)


</div>


# 6조 먹태팀 - 커넥듀 (Connectdu)

## 0. 서비스 요약

커넥듀 - AI 기반의 다국적 학습 보조 플랫폼

## 1. 주제 구분

- `E타입` - 경북대에 다니는 다양한 배경의 학우들을 위한 서비스

## 2. 팀원 소개

<div align="left">
   
| Full Stack | AI | FE | BE |
| --- | --- | --- | --- |
| <img src="https://avatars.githubusercontent.com/u/126179088?v=4" width="80px"/> |  <img src="https://avatars.githubusercontent.com/u/29157441?v=4" width="80px"/>|  <img src="https://avatars.githubusercontent.com/u/104586003?v=4" width="80px"/>|  <img src="https://avatars.githubusercontent.com/u/126085673?v=4" width="80px"/>|
| <div align="center">강태현</div> | <div align="center">김동주</div> | <div align="center">남소은</div> | <div align="center">이승빈</div> |
| <div align="center">[@KNU-K](https://github.com/KNU-K)</div> | <div align="center">[@rlaehd62](https://github.com/rlaehd62)</div> | <div align="center">[@2NNS-V](https://github.com/2NNS-V)</div> | <div align="center">[@LSBsity](https://github.com/LSBsity)</div> |

</div>

## 3. 시연 영상
- [**`Youtube`**](https://youtu.be/Mgg78njjYiU)

- [**`GitHub Organization`**](https://github.com/TEAM-MukTae)

- [**`FE Repository`**](https://github.com/TEAM-MukTae/fe)

- [**`BE Repository`**](https://github.com/TEAM-MukTae/be)

- [**`AI Repository`**](https://github.com/TEAM-MukTae/ai)

## 4. 서비스 소개
### 4-1. 서비스 개요
- 다양한 배경을 가진 학습자를 보조하기 위한 플랫폼이다.
- 실시간 음성인식을 통해 주요 언어에 대한 자막 및 번역을 제공한다.
- 음성 데이터를 수집하고 이를 AI로 요약 및 보정한다.
- AI를 기반으로 음성 데이터와 추가적인 PDF 문서를 통해 연습문제를 생성한다.
- 실시간 자막과 번역, 그리고 문서 요약을 통해 언어 장벽을 허물고 교육 접근성을 개선한다.
- 연습문제를 통해 학습 효율을 개선하고 전체적인 성취도를 향상 시킨다.

   
### 4-2. 타서비스와의 차별점
**4-2-1. 기존 서비스의 문제점**
- 전문 용어에 대한 전문성 부족
- 언어 번역 기능 부족
- 실시간으로 수업을 듣기 보다는, 녹음 후에 이후에 학습하는 용도

**4-2-2. 커넥듀의 차별점**
- RAG(검색증강생성)을 사용해 전문 용어에 대한 학습 효율 증진
- i18n을 사용해 사용자 언어에 따라 언어 다양성 제공
- 실시간 번역으로 수업 시간 이해도 증진

### 4-3. 구현 내용 및 결과물
**4-3-1. 실시간 번역 시스템**
- 사용자가 수업 시간에 음성 인식(Speach to Text) 기능을 통해 실시간 번역을 제공한다.
- 음성 인식이 완료되면, 녹음 파일을 생성해 복습할 수 있다.

**4-3-2. 인공지능 기반 퀴즈 생성 시스템**
- 사용자가 생성된 녹음 파일과 학습 자료를 업로드하면, 텍스트 인식 기능을 통해 퀴즈를 풀 수 있다.

**4-3-3. 인공지능 기반 요약 시스템**
- 사용자는 생성한 녹음 파일에 대한 스크립트와 요약본을 확인할 수 있다.

### 4-4. 구현 방식
**4-4-1. Infrastructure Architecture**

<img src="https://github.com/user-attachments/assets/d7925c92-4a15-401c-8b71-fc51817bf79a" width="300px"/>

**4-4-2. UI/UX Design**

<img src="https://github.com/user-attachments/assets/933526a5-6202-4c0f-8976-b612a0279b99" width="800px"/><br/>
<img src="https://github.com/user-attachments/assets/24386b3a-5eb0-4876-86f0-edac11effd0a" width="800px"/>

**4-4-3. Flow Diagram**

<img src="https://github.com/user-attachments/assets/3d11770d-d19d-466d-811b-808770e99b94" width="450px"/>


**4-4-4. Entity-Relationship Diagram**

<img src="https://github.com/user-attachments/assets/d1e5fe1f-c139-45fd-bd70-72851fb6bcbc" width="300px"/>



#### 4-5. 기술 스택
* BE
   * `java`, `spring boot`, `spring data jpa`, `spring kafka`, `spring security`
   
* FE
   * `typescript`, `react`, `recoil`, `tailwind`, `framer-motion`, `i8n` ,`axios`, `web speech api`
     
* AI
   *  `python`, `fastapi`, `kafka-python`, `openai`

* Message Broker
   * `Kafka`, `KafDrop`

* Externel Usage API
   * `Google Cloud Translation API`, `Kakao OAuth API`

* Infrastructure(with DevOps)
   * `AWS EC2`, `AWS S3`, `Docker`, `RDB`
 
* Database
   * `mysql`

* CI/CD pipeline
   * `git action`, `vercel`

## 향후 개선 혹은 발전 방안

1. 다국어 지원 확대 및 번역 품질 향상
- 커넥듀는 현재 한국어를 포함한 5개 언어를 지원하고 있지만, 향후 더 많은 유학생들의 요구를 충족시키기 위해 지원 언어를 단계적으로 확대할 계획입니다.
- 단순히 언어 수를 늘리는 것에 그치지 않고 각 언어별 전문 번역가와의 협업을 통해 번역의 품질을 지속적으로 개선할 것입니다. 특히 학술적 맥락과 전문 용어에 대한 정확한 번역을 제공하기 위해 분야별 전문가의 감수를 받을 계획입니다. 


2. AI 기반 퀴즈 생성 시스템의 고도화

- 현재 커넥듀의 AI 기반 퀴즈 생성 시스템은 기본적인 수준의 문제를 제공하고 있지만, 실제 대학 기출문제와 검증된 상용 문제집의 데이터를 확보하여 AI 모델에 학습시킬 계획입니다.
- 사용자 피드백 시스템을 구축하여 생성된 퀴즈의 적절성, 난이도, 학습 효과 등에 대한 평가를 지속적으로 수집하고, 데이터를 바탕으로 AI 모델을 지속적으로 튜닝하여, 각 학습자의 수준과 학습 목표에 맞는 최적화된 퀴즈를 제공할 것 입니다. 

3. 대학 협력 모델 구축

- 경북대학교를 시작으로 대구 경북권 대학교, 전국으로 서비스 확대를 확대하여 대학별 특성에 따른 맞춤 서비스 제공할 예정입니다.
- 각 대학의 학사 시스템과의 연동을 통해 수강 정보를 자동으로 반영하고, 교수진들이 직접 학습 자료를 업로드하거나 퀴즈를 생성할 수 있는 기능을 추가하여 보다 통합된 학습 경험을 제공할 계획입니다


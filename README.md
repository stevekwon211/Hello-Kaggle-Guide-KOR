# Hello Kaggle!:wave:

`Kaggle의 공식 문서`와 `캐글 가이드`라는 책을 읽고 `Kaggle`의 정의나 기본적인 사용법들에 대하여 정리해보았습니다.<br>
저처럼 이제 막 `Kaggle`을 접하는 분들에게 도움이 되었으면 합니다.<br>
수정해야할 부분이 있으면 `Issues`에 남겨주시면 감사하겠습니다.<br>

참고로 `Hello Kaggle!` 문서는 `Python 프로그래밍` 또는 `머신러닝 이론` 같은 것은 거의 다루지 않고 `Kaggle 사용법`에 집중하였습니다.<br>
프로그래밍이나 데이터 사이언스, 머신러닝 자료를 찾고 계신 분들을 위해 제가 도움을 받았던 링크를 몇 군데 남겨두겠습니다.<br>
- [DATA SCIENCE ROADMAP 2020](https://medium.com/@ArtisOne/data-science-roadmap-2020-b256fb948404)
- [datastacktv님의 data engineer roadmap](https://github.com/datastacktv/data-engineer-roadmap)
- [My Data Science Online Learning Journey on Croursera](https://www.kdnuggets.com/2020/11/data-science-online-learning-journey-coursera.html)
- [머신러닝 딥러닝 독학자료 모음 - teddylee777님의 machine-learning Repository](https://github.com/teddylee777/machine-learning)
- [Team-Neighborhood의 I want to study Data Science](https://github.com/Team-Neighborhood/I-want-to-study-Data-Science)
- [한걸음 한걸음, 데이터 과학자(Data Scientist)가 되는 방법](https://theorydb.github.io/dev/2020/04/12/dev-competition-how-to-become-data-scientist/)
<br>

## 목차
1. [Kaggle이란 무엇인가요?](#kaggle이란-무엇인가요)
    - [Kaggler? Kaggling?](#kaggler-kaggling)
    - [Competition외에 서비스나 특징들](#competition외에-서비스나-특징들)
    - [Kaggling을 위해 필요한 지식](#kaggling을-위해-필요한-지식)
    - [Kaggler가 되기 전에 준비해야 할 것](#kaggler가-되기-전에-준비해야-할-것)
<br>

2. [Kaggle은 어떻게 활용되나요?](#kaggle은-어떻게-활용되나요)
    - [데이터 분석을 위한 인프라로 활용하기](#데이터-분석을-위한-인프라로-활용하기)
    - [Notebook 활용하기](#notebook-활용하기)
    - [Dataset 활용하기](#dataset-활용하기)
    - [회사 연수에 활용하기](#회사-연수에-활용하기)
    - [Discussion 활용하기](#discussion-활용하기)
<br>

3. [Kaggle Competition?](#kaggle-competition)
    - [가장 일반적인 Competition인 Featured](#가장-일반적인-competition인-featured)
    - [연구목적의 Research](#연구목적의-research)
    - [학습용 Competition인 Getting Started](#학습용-competition인-getting-started)
    - [데이터 사이언티스트, 엔지어들의 Playground](#데이터-사이언티스트-엔지니어들의-playground)
    - [취업 기회를 얻을 수 있는 Recruitment](#취업-기회를-얻을-수-있는-recruitment)
    - [정기적으로 열리는 Annual Competition](#정기적으로-열리는-annual-competition)
    - [분석한 결과를 효과적으로 설명해야하는 Analytics](#분석한-결과를-효과적으로-설명해야하는-analytics)
<br>

4. [Kaggle 시작하기](#kaggle-시작하기)
    - [회원가입](#회원가입)
    - [Kaggle Courses 둘러보기](#kaggle-courses-둘러보기)
    - [Kaggle 등급](#kaggle-등급)
    - [메달](#메달)
    - [Kaggle Contributor 되기](#kaggle-contributor-되기)
    - [Kaggle Rankings](#잠깐)
<br>

5. [Notebook에 대하여](#notebook과-친해지기)
    - [Notebook 소개](#notebook에-대한-간단한-소개는-여기를-다시-읽어주세요)
    - [Notebook으로 할 수 있는 것은?](#notebook으로-할-수-있는-것은)
    - [Notebook 만들고 사용하기](#notebook-만들고-사용하기)
    - [Notebook의 다양한 설정](#notebook의-다양한-설정)
    - [Notebook에서 Data 불러오는 법](#notebook에서-data-불러오는-법)
    - [Notebook에서 외부 패키지 사용하기](#notebook에서-외부-패키지-사용하기)
    - [Notebook에서 Dataset 소스 코드 사용하기](#notebook에서-dataset-소스-코드-사용하기)
<br>

6. [Competitions과 Notebooks](#competitions과-notebooks)
    - [Competition Notebook에서 사용할 Data File 다루는 법](#competition-notebook에서-사용할-data-file-다루는-법)
<br>

#### 추가예정
7. [Competitions 세부 사항](#competition-세부-사항)
8. [Competition의 규칙](#competition의-규칙)
9. [Competition의 Data](#competition의-data)
10. [Competition에 사용된 최신 기술](#competition에-사용된-최신-기술)
11. [Kaggle의 Dataset과 API](#kaggle의-dataset과-api)
<br>

***

<br>

## Kaggle이란 무엇인가요?
- __`Kaggle`__ 은 데이터 분석 경진 대회를 주최하는 플랫폼입니다.
- 경진대회는 회사의 `연구 과제, 주요 서비스`를 위해 분석이 필요한 데이터를 제공해서 주최하는게 일반적입니다.
![1](https://user-images.githubusercontent.com/61633137/103594874-3c684d80-4f3d-11eb-9300-c33588266c63.png)
<br>

- __`인공지능, 머신러닝 붐`__ 이 일어나면서 참가자 수가 계속 증가해왔으며 2017년 `구글`의 모회사 __'Alphabet'__ 에 인수되기도 하였습니다.
- Alphabet의 인수 이후 Kaggle은 단순한 플랫폼이 아닌 데이터 사이언티스트, 엔지니어들에게 매우 중요한 사이트가 되었습니다.
<br>

### `Kaggler`? `Kaggling`?
- 마치 구글에서 검색하는 것을 __`Googling`__ 이라고 하는 것 처럼 <br>
  Kaggle의 사용자는 __`Kaggler`__, Kaggle에서 활동하거나 Competition에 참가하는 것은 __`Kaggling`__ 이라고 합니다.
<br>

### Competition외에 서비스나 특징들
- __`Jobs`__
  - Jobs를 원래 제공해왔으나 2020년 12월 22일 서비스를 종료했습니다.<br>
    간단하게 요약하자면 이용자 수가 적어서라네요.<br>
    자세한 내용은 https://www.kaggle.com/jobs-board-closed 여기서 읽어보시길 바랍니다.
<br>
    
- __[`Course`](https://www.kaggle.com/learn/overview)__
  ![image](https://user-images.githubusercontent.com/61633137/103596261-e0072d00-4f40-11eb-9e50-2315e734d267.png)
  - `Python`, `머신러닝`, `시각화` 등에 대한 실무, 실용적인 강의들을 제공합니다.
  - 체계적으로 배우지 못했거나 최신 기술이 아닌 강의를 공부했다면 Kaggle의 Course가 꽤 유용할 수 있습니다.
  - 또한 모든 강의들은 `영어`로 제공되고 `무료`이며 `수료증`을 제공합니다.
<br>
  
- __`영어`__
  - 전 세계의 데이터 사이언티스트들이 모이므로 기본적으로 `영어`를 사용합니다.
  - `Competition의 공지사항`, `데이터 세트(Dataset)`, `토론(Discussion)`도 영어로 이루어집니다. (영어 공부 필수!! 또는 `파파고..`)<br>
    아래는 Discussion과 Site Forum 사진입니다.
  ![image](https://user-images.githubusercontent.com/61633137/103596175-a59d9000-4f40-11eb-9e8c-90fc24e51347.png)
  - 실제로 Competition 입상자들의 프로필을 살펴보면 `미국`, `러시아`, `중국`, `인도`, `한국` 등 다양합니다.
<br>
  
- __`프로그래밍 언어`__
  - 일반적으로 __`Python`__ 과 __`R`__ 을 많이 사용합니다.
<br>

### Kaggling을 위해 필요한 지식
- |목적|필요한 지식|
  |------|-----|
  |Competition 참가|Python, R, 데이터 분석|
  |Competition 주최|데이터 분석, 영어|  
  |Kaggler와 토론|영어|
  |Course를 통한 학습|영어|
<br>

### Kaggler가 되기 전에 준비해야 할 것
- 필수: `인터넷`, `Python`, `R` 프로그래밍이 가능한 PC
- 권장: `GPU 탑재된 서버` or `워크스테이션`, 대용량의 `HDD` or `SSD`
<br>

***

<br>

## Kaggle은 어떻게 활용되나요?
### 데이터 분석을 위한 `인프라`로 활용하기
- Kaggle은 `웹 기반`으로 데이터 분석에 필요한 도구를 제공해줍니다.(Notebook)
- 다양한 Kaggler들과 커뮤니티를 이루고 있어 경쟁과 협력이 가능합니다.
<br>

### `Notebook` 활용하기
- Kaggle에서 제공하는 __`데이터 분석용 프로그래밍 환경`__ 입니다.
- SaaS 환경으로 Notebook에 작성한 코드를 서버에서 실행하는 방식입니다.
- 프로그래밍 환경을 제공해주므로 별도의 개발 환경 구축이 필요없습니다.(Python 설치, Anaconda 설치 등등 필요 X)
- __`Jupyter Notebook`__ 을 참고해 만들어져 비슷합니다.
- 기본적으로 `4Core CPU + 16GB RAM`을 제공합니다. `GPU 서버`는 `2Core CPU + GPU + 13GB RAM`을 제공합니다.<br>
  __`사용 횟수 제한없이 무료로 제공`__ 해주며 `GPU는 1주일에 30시간` 동안 사용할 수 있습니다.
<br>

### `Dataset` 활용하기
![image](https://user-images.githubusercontent.com/61633137/103597920-b18b5100-4f44-11eb-8f02-df689352a762.png)
- 머신러닝 기반의 데이터 분석 프로그램을 개발할 때 가장 먼저 해야하는 것은 __`Dataset`__ 을 준비하는 것입니다.
- 학술 목적으로 공개되었거나 Kaggler가 만들어 공개한 Dataset는 누구나 사용할 수 있습니다.
- 만약 공개하고 싶지 않은 Dataset이라면 __`Private`__ 설정을 통해 외부에는 공개하지 않을 수 있습니다.
- 한 번이라도 Dataset이나 Notebook을 `공개`로 설정하면 `Apache 2.0 License`가 적용되므로 신중하게 결정해야 합니다.
<br>

### `회사 연수`에 활용하기
- 책에 나온 예시: 신경망 기반 머신러닝 프로그래밍 작성 직원 연수
  - 1. Kaggle 회원 가입
  - 2. 직원들은 진행자의 Noteboook을 복사하고 실행할 준비
  - 3. Notebook의 신경망 모델 수정
  - 4. 수정한 모델의 실행 결과를 Competition에 제출하고 점수 확인
- 만약 Kaggle을 이용하지 않았다면?
  - 1. 연수용 컴퓨터에 개발 환경 구축
  - 2. 머신러닝 프로그램(신경망 모델) 예제 배포 
  - 3. 신경망 모델 실행 결과를 점수로 환산하여 평가하는 프로그램 작성
  - 4. 실행한 모델의 평가 점수 확인
  - 5. 신경망 모델 수정
  - 6. 실행 결과에 따라 점수가 달라지는 것을 확인
<br>

- Kaggle이 `개발 환경 구축`, `점수 확인`, `배포` 등의 점에서 훨씬 간편하고 비용이 덜 든다는 것을 알 수 있습니다.
<br>

### `Discussion` 활용하기
- 모르는 것이 있으면 메인 홈페이지의 __`Communities`__ , __`Site Forums`__ , 그리고 Competition마다 있는 __`Discusstion`__ 에 질문할 수 있습니다.<br>
- `Communities`
  ![image](https://user-images.githubusercontent.com/61633137/103608822-9548dd80-4f5f-11eb-8a55-626a9a0015bb.png)

- `Site Forums`
  ![image](https://user-images.githubusercontent.com/61633137/103608932-f2dd2a00-4f5f-11eb-8d5d-6f1761e61a1f.png)
<br>

***

<br>

## Kaggle Competition?
[Competitions Documentation](https://www.kaggle.com/docs/competitions)에서 몇 가지 내용을 참조하여 작성했습니다.
<br>

### 가장 일반적인 Competition인 `Featured`
![image](https://user-images.githubusercontent.com/61633137/103611173-0dfe6880-4f65-11eb-8141-aac631077c34.png)
- 난이도가 있으며 일반적으로 상업적인 목적을 가진 Competition들입니다.
- 대부분의 Kaggler들이 참여하며 지금까지 진행되었던 Competition들의 상금은 `$100`부터 많게는 `$1,500,000`까지도 있습니다.
<br>

### 연구목적의 `Research`
![image](https://user-images.githubusercontent.com/61633137/103611678-1d31e600-4f66-11eb-9e41-c972d26d3440.png)
- 연구적인 주제들을 주로 다루며 일반적으로 상금이나 보상은 주어지지 않습니다.(현재 진행중인 Research Competition들은 모두 상금이 있네요)
- 대신 덜 경쟁적이며 지적 호기심이 많은 Kaggler들과 토론해가며 연구를 할 수 있습니다.
<br>

### 학습용 Competition인 `Getting Started`
![image](https://user-images.githubusercontent.com/61633137/103609060-510a0d00-4f60-11eb-98e6-b42e4d2a8336.png)
- 여기에 나오는 Competition들은 초보자 대상의 학습용 Competition들입니다.
- 특히 __`Titanic: Machine Learning from Disaster`__ , __`House Prices: Advanced Regression Techniques`__ , __`Digit Recognizer`__ 이 3가지 Competition은 머신러닝에 입문한 분들에게   가장 많이 추천되고 도움이 되는 Competition들입니다.
<br>

### 데이터 사이언티스트, 엔지니어들의 `Playground`
![image](https://user-images.githubusercontent.com/61633137/103609928-45b7e100-4f62-11eb-992a-14a98dc190b3.png)
- 주로 데이터 사이언티스트와 엔지니어들이 흥미롭다고 느낄만한 주제들로 Competition이 열립니다.
- Playground라고 해서 난이도가 쉽진 않습니다. 보통 최근에 발표한 학술/기술적 문제나 공공 사회 문제도 다룹니다.
- 주최측에서 상금이나 보상을 제공하는 경우도 있습니다.
<br>

### 취업 기회를 얻을 수 있는 `Recruitment`
![image](https://user-images.githubusercontent.com/61633137/103611946-bc56dd80-4f66-11eb-8408-576df10506c3.png)
- 기업들이 주최하며 보상은 주로 Job Interview(면접) 기회입니다. Competition이 종료된 시점에 참가자들은 Resume(이력서)를 업로드할 수 있습니다.
<br>

### 정기적으로 열리는 `Annual Competition`
- Kaggle에는 정기적으로 열리는 Competition들이 몇 가지 있습니다. 현재 Kaggle의 에서 다음과 같은 내용을 확인할 수 있습니다.
  ![image](https://user-images.githubusercontent.com/61633137/103610665-04283580-4f64-11eb-9e75-b4f37e84c2bf.png)
<br>

### 분석한 결과를 효과적으로 설명해야하는 `Analytics`
- 이건 Documentation에 설명이 나와있지 않아서 현재 올라와있는 Analytics Competition들을 직접 읽어보고 작성했습니다.
- 각 Competition의 Evaluation과 Submission 형식을 읽어보니 Analytics의 채점 방식은 Notebook을 직접 제출하여 사람이 채점하는 방식으로 보여집니다.<br>
  분석한 데이터를 주최자의 요구사항에 맞게 설명해야 합니다. 마치 회사에서 프레젠테이션을 통해 경영진을 설득하는 것과 비슷해보입니다.
<br>

***

<br>

## Kaggle 시작하기
### `회원가입`
- Kaggle을 시작하기에 앞서 오른쪽 상단의 `Register` 버튼을 눌러서 회원가입을 먼저 진행해주셔야 합니다.
<br>

### Kaggle `Courses` 둘러보기
- 머신러닝이나 데이터 분석 공부가 충분하지 못한 분들은 위에서 소개했던 [`Courses`](https://www.kaggle.com/learn/overview)에서 필요한 부분을 공부하는 것도 좋은 방법입니다.
- 각 과정은 2~8개의 수업으로 구성되어 있고 다양한 실습 예제를 제공합니다.
<br>

[Kaggle Progression System](https://www.kaggle.com/progression)을 참조해서 작성했습니다.<br>
`Contributer`가 되는 법에 대해 설명하기 전에 `Kaggle 등급`과 `메달`에 대한 설명을 먼저 하겠습니다.

### Kaggle `등급`
- Kaggle에는 Progression System이 있는데 쉽게 이야기해서 `Kaggler 등급`입니다.<br>
  이 등급은 데이터 사이언티스트로써 어느정도의 실력을 가졌는지 가늠할 수 있는 좋은 지표입니다.<br>
  또한 자신이 얼마나 성장했는지를 직관적으로 보여주기도 합니다. 
- Kaggle 등급은 다음과 같이 5단계로 나뉘어지며 각 등급을 달성하기 위한 조건도 제시되어 있습니다.
  - `Novice`<br>
    ![image](https://user-images.githubusercontent.com/61633137/103615154-689bc280-4f6d-11eb-9893-a3336cd8c00b.png)
  <br>
  
  - `Contributor`<br>
    ![image](https://user-images.githubusercontent.com/61633137/103615214-85d09100-4f6d-11eb-8ed2-60415fdcc0ad.png)
  <br>
  
  - `Expert`<br>
    ![image](https://user-images.githubusercontent.com/61633137/103615347-c9c39600-4f6d-11eb-8dc6-6525f5bf35a6.png)
  <br>
  
  - `Master`<br>
    ![image](https://user-images.githubusercontent.com/61633137/103615383-d9db7580-4f6d-11eb-8705-c983f7a70e1e.png)
  <br>
  
  - `Grandmaster`<br>
    ![image](https://user-images.githubusercontent.com/61633137/103615428-e9f35500-4f6d-11eb-839c-c1af9c1494ed.png)
  <br>
  
- 또한 위 사진들에서 볼 수 있듯이 Kaggle 등급은 `Competitions`, `Datasets`, `Notebooks`, `Discussion` 각 분야 별로 다르게 부여됩니다.
- 오른쪽 위 계정 아이콘을 누른 후 `My Profile`을 선택해서 프로필 페이지로 넘어갑니다.<br>
  그럼 본인의 프로필 정보와 Kaggle 활동 내용 및 등급을 확인할 수 있습니다.<br>
<br>

### `메달`
- 간단히 이야기해서 메달은 Kaggler들의 각 분야에서의 활동 성과를 보여줍니다. 
  - `Competition`에서 훌륭한 결과를 얻은 Kaggler
  - 인기가 많은 `Notebook`을 작성하고 공유하는 Kaggler
  - 유용한 `Dataset`을 공유하는 Kaggler
  - 좋은 `Comment`를 작성하는 Kaggler
<br>

- `Contributer` 등급은 해당하는 조건을 만족하면 되지만 `Expert` 부터는 각 분야에 해당하는 조건에 요구하는 메달을 모아야 합니다.
- `Competitions`의 경우 참가하는 팀 수에 따라 메달의 수여 기준도 다음과 같이 달라집니다.<br>
  ![image](https://user-images.githubusercontent.com/61633137/103616627-1d36e380-4f70-11eb-8d7b-c026270fab11.png)
<br>

- `Datasets`, `Notebooks`, `Discussion`은 Vote 숫자로 평가합니다. Vote 숫자가 높을 수록 많은 Kaggler들에게 추천을 받았다는 의미입니다.<br>
  ![image](https://user-images.githubusercontent.com/61633137/103617270-52900100-4f71-11eb-9760-7e520ffddd4b.png)
- 유의해야할 사항은 각 부분의 게시물별로 수여되는 메달의 종류는 하나입니다.<br>
  예를 들어서 `Dataset`에 올린 게시물이 20 Votes를 받았다면 동메달은 없어지고 은메달을 받는 것입니다.
<br>

### Kaggle `Contributor` 되기
#### 1.사용자 프로필 정보 추가하기
- 본인의 프로필에 들어가서 Edit Profile을 클릭하고 다음 내용을 입력합니다.
  - `자기소개 (bio)`
  - `직업 (Occupation)`
  - `소속 조직 (Organization)`
  - `거주 도시 (City)`
- 그 외에 `프로필 이미지`, `SNS` 등은 자유롭게 설정하시면 됩니다.
<br>

#### 2. SMS 인증하기 (SMS verify your account)
- 프로필 화면에서 `Phone Verification`을 클릭합니다.
- `국가코드 (Country Code)`, `전화번호 (Phone Number)`, `로봇이 아닙니다` 박스에 체크를 한 후 `Send code`를 클릭합니다.
- 전송된 코드를 입력하고 `Verify`를 클릭하면 인증이 완료됩니다.
<br>

#### 3. Script 실행하기 (Run 1 script)
- `Course`에서 강의를 진행하거나 직접 `Notebook`을 생성하여 아무 코드나 실행해보면 달성할 수 있습니다.
- `4. Competition에 참가하기`에도 실행하는 과정이 있으니 건너뛰어도 괜찮습니다.
<br>

#### 4. Competition에 참가하기 (Make 1 competition or task submission)
- `Getting Started` 카테고리에 있는 Competition을 하나 고릅니다.
- 들어가보면 화면 중간 정도에 아래와 같은 메뉴를 보실 수 있습니다.<br>
![image](https://user-images.githubusercontent.com/61633137/103619281-cbdd2300-4f74-11eb-8c00-840110e018ce.png)
- 여기서 `Notebooks`를 클릭하고 다른 사람들이 작성한 Notebook들을 구경해봅니다.
  <br>
  
- 원하는 Notebook을 하나 골라서 열어보면 오른쪽 위에 ![image](https://user-images.githubusercontent.com/61633137/103619428-12cb1880-4f75-11eb-9ec9-435c40a13160.png)
  버튼이 보일 것입니다. 이 버튼을 클릭해서 Notebook을 복사합니다.
  <br>
  
- 복사가 완료되면 다시 오른쪽 위에 있는 `Save Version`을 클릭합니다.
  - `Version Name`: 원하는 이름을 입력할 수 있습니다.
  - `Version Type`: `Quick Save` 또는 `Save & Run All (Commit)`, 두 가지 옵션이 있는데 `Quick Save`는 저장만하고 실행은 하지 않으며 `Save & Run All (Commit)`은 실행도 합니다.
<br>

- 여기서 `Save & Run All (Commit)`을 클릭하고 `Save` 버튼을 누릅니다.
<br>

- 다시 프로필로 돌아가서 `Notebooks`를 클릭하면 방금 복사한 Notebook을 확인할 수 있습니다.<br>
  이 노트북을 클릭하면 오른쪽 메뉴 중에 `Output`이 있습니다.<br> 
  `Output`을 누르면 볼 수 있는 `Submission.csv`(Submission 파일의 이름은 다를 수도 있습니다)를 선택하고 오른쪽에 있는 `Submit to Competition`을 클릭합니다.
<br>

- 이제 `Leaderboard` 메뉴로 화면이 옮겨지고 제출된 파일이 자동으로 채점이 됩니다.<br>
  채점이 끝나면 점수를 확인할 수 있고 `Jump to your position on the leaderboard`를 클릭해 자신의 순위를 확인할 수 있습니다.
<br>

#### 5. 댓글 달고 다른 사람의 게시물이나 댓글에 Upvote 하기 (Make 1 comment & Cast 1 upvote)
- `Discussion`에서 자신이 원하는 Topic에 들어가서 관심있는 글을 클릭합니다. (`Site Forums`의 `Getting Started`에 들어가보는 것을 추천드립니다.)
- 글을 잘 읽어보고 `댓글`을 작성합니다. 글이 유용하거나 마음에 들었다면 `Vote`도 눌러줍시다.
<br>

#### 6. Kaggle `Contributor` 되기 완료!

#### 잠깐!
- 한 가지 내용을 더 추가하겠습니다. 바로 [Kaggle Rankings](https://www.kaggle.com/rankings)입니다.
- `Competitions`, `Datasets`, `Notebooks`, `Discussion` 네 분야 별로 순위를 확인할 수 있습니다.
- 아래 사진은 `Competitions` 분야의 순위를 보여주고 있습니다. 또한 그 분야에 각 등급별로 몇 명이나 있는지 확인도 가능합니다.
  ![image](https://user-images.githubusercontent.com/61633137/103715609-6c2e5880-5004-11eb-8970-9965f8089d15.png)
<br>

***

<br>

## Notebook과 친해지기
### [Notebook에 대한 간단한 소개는 여기를 다시 읽어주세요!](#notebook-활용하기)
<br>

### `Notebook`으로 할 수 있는 것은?
- 데이터 분석용 프로그래밍이 주 목적이며 작성된 프로그램은 캐글 서버에서 실행됩니다.
- `Competition`에 제출하거나 `Notebook`을 `Kaggler`들과 공유할 수 있습니다. 공유되는 `Notebook`중에는 오직 교육 또는 기술을 알려주기위한 목적인 것도 있습니다.
- `코드용 셀` 과 `마크다운 셀`을 활용하여 코드, 코드에 대한 설명(텍스트, 이미지 등)을 작성할 수 있습니다. <br>
  [마크다운(Markdown) 사용법](https://gist.github.com/ihoneymon/652be052a0727ad59601)<br>
  [마크다운 emoji-cheat-sheet](https://github.com/ikatyang/emoji-cheat-sheet)<br>
  위 두가지 링크는 제가 처음 마크다운을 사용하면서 참고했고 이모지는 지금도 필요할 때마다 가끔식 보고있습니다.
<br>

### `Notebook` 만들고 사용하기
- `Notebook` 메뉴에 들어가서 오른쪽 상단을 보면 ![image](https://user-images.githubusercontent.com/61633137/103716652-f081db00-5006-11eb-9368-e3bbe2795bbc.png) 이런 버튼이 있을텐데 클릭해줍니다.
<br>

- `Kaggle Notebook`은 `Script`와 `Notebook`, 두 가지 타입을 선택할 수 있습니다.
  - `Script`는 일반적으로 사용하는 코드 편집기에 코드를 작성하고 실행하는 방식입니다.
  - `Notebook`은 `Jupyter Notebook`과 비슷한 인터랙티브 개발 환경입니다. 셀을 나누어서 원하는 부분의 코드만 실행할 수 있는 특징이 있습니다.
<br>

- 왼쪽 상단에 `File`을 누르고 `Editor Type`에 커서를 대면 타입을 고를 수 있습니다. 또한 `Language`에서 `Python`과 `R`중에 사용할 언어를 고를 수 있습니다.<br>
  ![스크린샷(1)](https://user-images.githubusercontent.com/61633137/103716793-38a0fd80-5007-11eb-854c-f709e9ac911b.png)
<br>

- 왼쪽 상단에 아래 사진과 같이 생긴 칸을 누르면 이름을 변경할 수 있습니다.<br>
  ![image](https://user-images.githubusercontent.com/61633137/103717015-c0870780-5007-11eb-9fb8-13c501956cb2.png)
<br>

- 처음 `Notebook`을 생성하면 다음과 같은 코드가 보일 것입니다.
  ```python
  # This Python 3 environment comes with many helpful analytics libraries installed
  # It is defined by the kaggle/python Docker image: https://github.com/kaggle/docker-python
  # For example, here's several helpful packages to load

  import numpy as np # linear algebra
  import pandas as pd # data processing, CSV file I/O (e.g. pd.read_csv)

  # Input data files are available in the read-only "../input/" directory
  # For example, running this (by clicking run or pressing Shift+Enter) will list all files under the input directory

  import os
  for dirname, _, filenames in os.walk('/kaggle/input'):
      for filename in filenames:
          print(os.path.join(dirname, filename))

  # You can write up to 20GB to the current directory (/kaggle/working/) that gets preserved as output when you create a version using "Save & Run All" 
  # You can also write temporary files to /kaggle/temp/, but they won't be saved outside of the current session
  ```
  위 코드는 `Python`의 `Numpy`와 `Pandas` 라이브러리를 불러온 후, 파일을 가져올 디렉터리를 `/kaggle/input`으로 지정한 것입니다.
<br>

- `Notebook`에 `Hello Kaggle!`을 출력해보겠습니다. 아무 코드셀에 커서를 대면 `+ Code` 버튼을 볼 수 있는데 눌러주도록 합니다.
- 그러고 나서 다음과 같이 작성해줍니다.<br>
  ![image](https://user-images.githubusercontent.com/61633137/103717568-2c1da480-5009-11eb-94d3-486db9f4b4eb.png)
<br>

- 왼쪽 상단의 ![image](https://user-images.githubusercontent.com/61633137/103718200-89195a80-5009-11eb-83a9-efa581ca645a.png) 이 재생버튼을 눌러주거나<br>
  현재 실행시키고 싶은 코드 셀로 가서 `Ctrl + Enter` 또는 `Shift + Enter` 입력해서 코드를 실행합니다. 그러면 다음과 같이 출력이 될 것입니다.<br>
  ![image](https://user-images.githubusercontent.com/61633137/103717489-f4166180-5008-11eb-88b8-85936bb31044.png)
<br>

- 셀에서 볼 수 있는 버튼들의 각 기능들입니다.
  -![image](https://user-images.githubusercontent.com/61633137/103721394-e369e980-5010-11eb-8df6-a5f77b67caf3.png) : 셀 위치를 한 칸 앞으로 올립니다.
  -![image](https://user-images.githubusercontent.com/61633137/103721428-f7155000-5010-11eb-86f7-3a0e8ccff5af.png) : 셀 위치를 한 칸 아래로 내립니다.
  -![image](https://user-images.githubusercontent.com/61633137/103721456-085e5c80-5011-11eb-9768-24161e8b6f4e.png) : 해당 셀을 삭제합니다.
  -![image](https://user-images.githubusercontent.com/61633137/103721476-17450f00-5011-11eb-92ba-84e80c437c8d.png)/![image](https://user-images.githubusercontent.com/61633137/103721509-2deb6600-5011-11eb-88ed-979cd05bbb7b.png) : 해당 셀을 숨기거나 나타냅니다.
  -![image](https://user-images.githubusercontent.com/61633137/103721551-48254400-5011-11eb-98ef-66aaa3e6a3c8.png) : 다음과 같은 부가 기능을 제공합니다.<br>
   ![image](https://user-images.githubusercontent.com/61633137/103721556-49ef0780-5011-11eb-8abb-45061ffa7de0.png)
<br>

### `Notebook`의 다양한 설정 
- `공개`&`비공개` 설정하기
  - `Notebook`은 다른 `Kaggler`들에게 공유하기 위해 공개할 수 있습니다. 하지만 본인만 알고싶다거나 팀으로 활동할 때에는 `비공개`, `특정 사용자에게 공유`같은 설정을 할 수 있습니다.
  - 오른쪽 상단에 있는 `Share` 버튼을 누르면 공개 또는 비공개를 설정하는 창이 열립니다.
  - `Privacy`를 `Public`으로 설정하면 `Apache 2.0 License` 적용과 함께 공개가 됩니다.
  - `Colaborators`에서 사용자를 검색해 공동 작업자로 추가할 수 있습니다.
<br>

- `Settings` 설명
  - `Language` : `Python`과 `R` 중에 사용할 프로그래밍 언어를 설정할 수 있습니다.
  - `Environment` : `Docker` 이미지를 설정할 수 있습니다. `Original`은 `Notebook`을 만들 때 직접 개발 환경을 설정하는 것이고 `Latest Available`은 `Kaggle`이 제공하는 최신 개발 환경을 사용하는 옵션입니다.
  - `Accelerator` : `GPU` 또는 `TPU`를 사용할지 설정할 수 있습니다.
  - `GPU/TPU Quota` : `GPU` 및 `TPU` 사용 시간와 사용량을 보여줍니다.
  - `Internet` : 인터넷 연결 여부를 설정할 수 있습니다.<br>
    `Internet`을 `On`으로 설정하면 특정 패키지를 설치할 수 있습니다. 또한 구글 계정을 이용해 `GCP (Google Cloud Platform)`의 `BigQuery`, `Cloud Storage`, `AutoML` 서비스를 사용할 수 있습니다.
<br>

### `Notebook`에서 `Data` 불러오는 법
- `Kaggle Notebook`은 `Competition Data` 뿐만 아니라 공유되고 있는 다양한 `Dataset`을 이용할 수 있습니다.<br>
  이런 경우에는 별도의 파일을 `Notebook`에서 사용할 수 있도록 설정해주어야 합니다.
<br>

- 1. 새로운 `Notebook`을 만들어서 하는 방법
    - 자신이 사용하길 원하는 `Dataset`에 가면 ![image](https://user-images.githubusercontent.com/61633137/103732584-086b5600-502b-11eb-9d12-06d4a77914b8.png) 이런 버튼을 볼 수 있는데 `New Notebook`을 누르면 파일이 자동으로 설정됩니다.<br>
<br>

- 2. 기존의 `Notebook`에 추가하는 방법
    - 현재 갖고있는 `Notebook`에 새로운 데이터를 추가하려면 우선 `Notebook`으로 접속합니다.<br>
      그리고 오른쪽 상단에 있는 ![image](https://user-images.githubusercontent.com/61633137/103732714-4d8f8800-502b-11eb-8909-4825d3eabec4.png) `+ Add Data` 버튼을 클릭합니다.<br>
      그러고나면 창이 하나 나타나는데 거기서 원하는 `Dataset`을 검색한 후 `Add`를 누르면 됩니다. 
<br>

- 3. 직접 업로드하는 방법
    - `Data` 메뉴에 들어가서 오른쪽 상단을 보면 ![image](https://user-images.githubusercontent.com/61633137/103733211-8b40e080-502c-11eb-8088-69e4bbf28e72.png) `+ New Data` 버튼이 있는데 이것을 클릭합니다.<br>
      그리고 `Enter Dataset Title`에 이름을 입력한 뒤 `Select Files to Upload`를 눌러서 파일을 업로드합니다. (zip이나 tar.gz같은 압축 파일 형식도 가능합니다.)<br>
      마지막으로 `Create`을 눌러서 `Dataset`을 업로드합니다. 이렇게 업로드한 `Dataset`을 i이나 ii의 방식으로 불러와서 사용하면 됩니다.
<br>

- 4. 다른 `Notebook`의 출력 데이터를 사용하는 방법
    - ii의 방법을 따라하면 창이 하나 나타나는데 거기서 `Kernel Ouput Files` 탭을 클릭하면 다른 `Notebook`의 출력 데이터를 사용할 수 있습니다.
<br>

### `Notebook`에서 외부 패키지 사용하기
- `pip`로 설치할 수 있는 외부 패키지는 `Notebook`의 하단에 있는 `Console`을 클릭해서 `pip install package_name`과 같이 설치할 수 있습니다.<br>
   ![image](https://user-images.githubusercontent.com/61633137/103733887-153d7900-502e-11eb-9660-12bf25592e96.png)
<br>

- 또한 다음 두 가지 예시처럼 코드 셀에서 직접 `pip`를 사용할 수도 있습니다.
  ```python
  !pip install package_name
  ```
  ```python
  import os
  os.system('pip install package_name')
  ```
<br>

### `Notebook`에서 `Dataset` 소스 코드 사용하기
- 만약 `hello_kaggle` 이라는 패키지를 포함한 `example dataset`을 `Notebook`에 추가하면 ../input/example-dataset/hello_kaggle 디렉터리를 추가하면됩니다.<br>
  추가하는 코드는 다음과 같습니다.
  ```python
  import sys
  sys.path.append("../input/example-dataset/hello_kaggle")
  ```
<br>

***

<br>

## Competitions과 Notebooks
### `Notebook`은 데이터 분석 `Competition` 말고 어디에 사용되나요?
- 일반적으로 입상이 목표라면 `Competition`이 종료된 후 `Notebook`을 공개하게 됩니다.<br>
  하지만 `Competition`이 진행되고 있을 때에도 `Kaggler`들과 토론을 할 수 있는 환경도 조성되어 있습니다.
<br>

### `Competition Notebook`에서 사용할 `Data File` 다루는 법
- `Competition`을 진행할 때 `Notebook`의 오른쪽 상단을 보면 `Data` 탭이 있습니다. 눌러보면 3가지의 파일이 있을 것인데 각 파일에 대한 설명은 다음과 같습니다.
  - `train.csv` : 정답 레이블이 있는 학습용 데이터입니다.
  - `test.csv` : 정답 레이블이 없는 테스트용 데이터입니다.
  - `sample_submission.csv` : 제출용 데이터 예입니다.
<br>

- `Competition`의 `Data` 메뉴를 보면 각 파일이 어떤 데이터가 담겨 있는지 확인할 수 있습니다.<br>
  예시로 `Titanic - Machine Learning from Disaster`를 보겠습니다.<br>
  ![image](https://user-images.githubusercontent.com/61633137/103719565-9e43b880-500c-11eb-95ff-67b5cda88821.png)<br>
  위 사진에서 [Data](https://www.kaggle.com/c/titanic/data?select=gender_submission.csv) 메뉴를 클릭하면 다음과 같이 Overview를 읽어볼 수 있고<br>
  ![image](https://user-images.githubusercontent.com/61633137/103719731-00042280-500d-11eb-8638-b0f543c65171.png)<br>
  더 아래로 내려가보면 다음과 같이 각 파일을 선택해 데이터를 확인해볼 수 있으며 다운로드도 가능합니다.<br>
  ![image](https://user-images.githubusercontent.com/61633137/103719767-17431000-500d-11eb-9e20-e36dccdadbb4.png)<br>

- 위 파일들을 이용해서 모델을 작성 및 제출할 csv 파일을 생성했다고 가정하고 제출하는 방법을 다루어보겠습니다.<br> 
  ([4-competition에-참가하기](#4-competition에-참가하기-make-1-competition-or-task-submission)에서도 같은 내용이 설명되어 있습니다.)
  - `Notebook` 화면의 오른쪽 상단에 있는 `Save Version`을 클릭합니다. (만약 코드를 실행하지 않은 상태라면 `Save & Run All (Commit)`을 클릭하면 됩니다.
  - `Save & Run All (Commit)`에서 `Commit`은 현재 제가 문서를 작성하고 있는 `Github`의 `Git`과 같은 의미입니다.<br>
    그래서 `Kaggle Notebook`은 이전에 작성했던 소스 코드의 버전을 참조할 수 있습니다.
    
- 이제 프로필로 돌아가서 `Notebooks`를 클릭하면 방금 저장한 Notebook을 확인할 수 있습니다.<br>
  이 노트북을 클릭하면 오른쪽 메뉴 중에 `Output`이 있습니다.<br> 
  `Output`을 누르면 볼 수 있는 `Submission.csv`를 선택하고 오른쪽에 있는 `Submit to Competition`을 클릭합니다.
<br>

- 이제 `Leaderboard` 메뉴로 화면이 옮겨지고 제출된 파일이 자동으로 채점이 됩니다.<br>
  채점이 끝나면 점수를 확인할 수 있고 `Jump to your position on the leaderboard`를 클릭해 자신의 순위를 확인할 수 있습니다.
<br>

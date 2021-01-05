# 
`Kaggle의 공식 문서`과 `캐글 가이드`라는 책을 읽고 나름대로 정리해보았습니다.<br>
저처럼 이제 막 Kaggle을 접하는 분들에게 도움이 됐으면 합니다.<br>
수정해야할 부분이 있으면 `Issues`에 남겨주시면 감사하겠습니다.<br>

## 목차
1. [Kaggle이란 무엇인가요?](#kaggle이란-무엇인가요)
2. [Kaggle은 어떻게 활용되나요?](#kaggle은-어떻게-활용되나요)
3. [Kaggle Competition?](#kaggle-competition)
4. [Kaggle 시작하기](#kaggle-시작하기)

#### 추가예정
5. [Notebook이란 무엇인가요?](#notebook이란-무엇인가요)
6. [Notebook 사용하는 법](#notebook-사용하는-법)
7. [Competitions with Notebooks](#competitions-with-notebooks)
8. [Competitions 세부 사항](#competition-세부-사항)
9. [Competition의 규칙](#competition의-규칙)
10. [Competition의 Data](#competition의-data)
11. [Competition에 사용된 최신 기술](#competition에-사용된-최신-기술)
12. [Kaggle의 Dataset과 API](#kaggle의-dataset과-api)
13. [Kaggle에서 자주 사용하는 LightGBM](#kaggle에서-자주-사용하는-lightgbm)
14. [Kaggle에서 자주 사용하는 fast.ai](#kaggle에서-자주-사용하는-fast.ai)
<br>

***

<br>

# Kaggle이란 무엇인가요?
- __`Kaggle`__ 은 데이터 분석 경진 대회를 주최하는 플랫폼입니다.
- 경진대회는 회사의 `연구 과제, 주요 서비스`를 위해 분석이 필요한 데이터를 제공해서 주최하는게 일반적입니다.
![1](https://user-images.githubusercontent.com/61633137/103594874-3c684d80-4f3d-11eb-9300-c33588266c63.png)
<br>

- __`인공지능, 머신러닝 붐`__ 이 일어나면서 참가자 수가 계속 증가해왔으며 2017년 `구글`의 모회사 __'Alphabet'__ 에 인수되기도 하였습니다.
- Alphabet의 인수 이후 Kaggle은 단순한 플랫폼이 아닌 데이터 사이언티스트, 엔지니어들에게 매우 중요한 사이트가 되었습니다.
<br>

## `Kaggler`? `Kaggling`?
- 마치 구글에서 검색하는 것을 __`Googling`__ 이라고 하는 것 처럼 <br>
  Kaggle의 사용자는 __`Kaggler`__, Kaggle에서 활동하거나 Competition에 참가하는 것은 __`Kaggling`__ 이라고 합니다.
<br>

## Competition외에 서비스나 특징들
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

## Kaggling을 위해 필요한 지식
- |목적|필요한 지식|
  |------|-----|
  |Competition 참가|Python, R, 데이터 분석|
  |Competition 주최|데이터 분석, 영어|  
  |Kaggler와 토론|영어|
  |Course를 통한 학습|영어|
<br>

## Kaggler가 되기 전에 준비해야 할 것
- 필수: `인터넷`, `Python`, `R` 프로그래밍이 가능한 PC
- 권장: `GPU 탑재된 서버` or `워크스테이션`, 대용량의 `HDD` or `SSD`
<br>

***

<br>

# Kaggle은 어떻게 활용되나요?
## 데이터 분석을 위한 `인프라`로 활용하기
- Kaggle은 `웹 기반`으로 데이터 분석에 필요한 도구를 제공해줍니다.(Notebook)
- 다양한 Kaggler들과 커뮤니티를 이루고 있어 경쟁과 협력이 가능합니다.
<br>

## `Notebook` 활용하기
- Kaggle에서 제공하는 __`데이터 분석용 프로그래밍 환경`__입니다.
- SaaS 환경으로 Notebook에 작성한 코드를 서버에서 실행하는 방식입니다.
- 프로그래밍 환경을 제공해주므로 별도의 개발 환경 구축이 필요없습니다.(Python 설치, Anaconda 설치 등등 필요 X)
- __`Jupyter Notebook`__ 을 참고해 만들어져 비슷합니다.
- 기본적으로 `4Core CPU + 16GB RAM`을 제공합니다. `GPU 서버`는 `2Core CPU + GPU + 13GB RAM`을 제공합니다.<br>
  __`사용 횟수 제한없이 무료로 제공`__ 해주며 `GPU는 1주일에 30시간` 동안 사용할 수 있습니다.
<br>

## `Dataset` 활용하기
![image](https://user-images.githubusercontent.com/61633137/103597920-b18b5100-4f44-11eb-8f02-df689352a762.png)
- 머신러닝 기반의 데이터 분석 프로그램을 개발할 때 가장 먼저 해야하는 것은 __`Dataset`__ 을 준비하는 것입니다.
- 학술 목적으로 공개되었거나 Kaggler가 만들어 공개한 Dataset는 누구나 사용할 수 있습니다.
- 만약 공개하고 싶지 않은 Dataset이라면 __`Private`__ 설정을 통해 외부에는 공개하지 않을 수 있습니다.
- 한 번이라도 Dataset이나 Notebook을 `공개`로 설정하면 `Apache 2.0 License`가 적용되므로 신중하게 결정해야 합니다.
<br>

## `회사 연수`에 활용하기
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

## `Discussion` 활용하기
- 모르는 것이 있으면 메인 홈페이지의 __`Communities`__ , __`Site Forums`__ , 그리고 Competition마다 있는 __`Discusstion`__ 에 질문할 수 있습니다.<br>
- `Communities`
  ![image](https://user-images.githubusercontent.com/61633137/103608822-9548dd80-4f5f-11eb-8a55-626a9a0015bb.png)

- `Site Forums`
  ![image](https://user-images.githubusercontent.com/61633137/103608932-f2dd2a00-4f5f-11eb-8d5d-6f1761e61a1f.png)
<br>

***

<br>

# Kaggle Competition?
[Competitions Documentation](https://www.kaggle.com/docs/competitions)에서 몇 가지 내용을 참조하여 작성했습니다.
<br>

## 가장 일반적인 Competition인 `Featured`
![image](https://user-images.githubusercontent.com/61633137/103611173-0dfe6880-4f65-11eb-8141-aac631077c34.png)
- 난이도가 있으며 일반적으로 상업적인 목적을 가진 Competition들입니다.
- 대부분의 Kaggler들이 참여하며 지금까지 진행되었던 Competition들의 상금은 `$100`부터 많게는 `$1,500,000`까지도 있습니다.
<br>

## 연구목적의 `Research`
![image](https://user-images.githubusercontent.com/61633137/103611678-1d31e600-4f66-11eb-9e41-c972d26d3440.png)
- 연구적인 주제들을 주로 다루며 일반적으로 상금이나 보상은 주어지지 않습니다.(현재 진행중인 Research Competition들은 모두 상금이 있네요)
- 대신 덜 경쟁적이며 지적 호기심이 많은 Kaggler들과 토론해가며 연구를 할 수 있습니다.
<br>

## 학습용 Competition인 `Getting Started`
![image](https://user-images.githubusercontent.com/61633137/103609060-510a0d00-4f60-11eb-98e6-b42e4d2a8336.png)
- 여기에 나오는 Competition들은 초보자 대상의 학습용 Competition들입니다.
- 특히 __`Titanic: Machine Learning from Disaster`__ , __`House Prices: Advanced Regression Techniques`__ , __`Digit Recognizer`__ 이 3가지 Competition은 머신러닝에 입문한 분들에게   가장 많이 추천되고 도움이 되는 Competition들입니다.
<br>

## 데이터 사이언티스트, 엔지니어들의 `Playground`
![image](https://user-images.githubusercontent.com/61633137/103609928-45b7e100-4f62-11eb-992a-14a98dc190b3.png)
- 주로 데이터 사이언티스트와 엔지니어들이 흥미롭다고 느낄만한 주제들로 Competition이 열립니다.
- Playground라고 해서 난이도가 쉽진 않습니다. 보통 최근에 발표한 학술/기술적 문제나 공공 사회 문제도 다룹니다.
- 주최측에서 상금이나 보상을 제공하는 경우도 있습니다.
<br>

## 취업 기회를 얻을 수 있는 `Recruitment`
![image](https://user-images.githubusercontent.com/61633137/103611946-bc56dd80-4f66-11eb-8408-576df10506c3.png)
- 기업들이 주최하며 보상은 주로 Job Interview(면접) 기회입니다. Competition이 종료된 시점에 참가자들은 Resume(이력서)를 업로드할 수 있습니다.
<br>

## 정기적으로 열리는 `Annual Competition`
- Kaggle에는 정기적으로 열리는 Competition들이 몇 가지 있습니다. 현재 Kaggle의 에서 다음과 같은 내용을 확인할 수 있습니다.
  ![image](https://user-images.githubusercontent.com/61633137/103610665-04283580-4f64-11eb-9e75-b4f37e84c2bf.png)
<br>

## 분석한 결과를 효과적으로 설명해야하는 `Analytics`
- 이건 Documentation에 설명이 나와있지 않아서 현재 올라와있는 Analytics Competition들을 직접 읽어보고 작성했습니다.
- 각 Competition의 Evaluation과 Submission 형식을 읽어보니 Analytics의 채점 방식은 Notebook을 직접 제출하여 사람이 채점하는 방식으로 보여집니다.<br>
  분석한 데이터를 주최자의 요구사항에 맞게 설명해야 합니다. 마치 회사에서 프레젠테이션을 통해 경영진을 설득하는 것과 비슷해보입니다.
<br>

***

<br>

# Kaggle 시작하기
## `회원가입`
- Kaggle을 시작하기에 앞서 오른쪽 상단의 `Register` 버튼을 눌러서 회원가입을 먼저 진행해주셔야 합니다.
<br>

## Kaggle `Courses` 둘러보기
- 머신러닝이나 데이터 분석 공부가 충분하지 못한 분들은 위에서 소개했던 [`Courses`](https://www.kaggle.com/learn/overview)에서 필요한 부분을 공부하는 것도 좋은 방법입니다.
- 각 과정은 2~8개의 수업으로 구성되어 있고 다양한 실습 예제를 제공합니다.
<br>

[Kaggle Progression System](https://www.kaggle.com/progression)을 참조해서 작성했습니다.<br>
`Contributer`가 되는 법에 대해 설명하기 전에 `Kaggle 등급`과 `메달`에 대한 설명을 먼저 하겠습니다.

## Kaggle `등급`
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

## `메달`
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

## Kaggle `Contributor` 되기
### 1.사용자 프로필 정보 추가하기
- 본인의 프로필에 들어가서 Edit Profile을 클릭하고 다음 내용을 입력합니다.
  - `자기소개 (bio)`
  - `직업 (Occupation)`
  - `소속 조직 (Organization)`
  - `거주 도시 (City)`
- 그 외에 `프로필 이미지`, `SNS` 등은 자유롭게 설정하시면 됩니다.
<br>

### 2. SMS 인증하기 (SMS verify your account)
- 프로필 화면에서 `Phone Verification`을 클릭합니다.
- `국가코드 (Country Code)`, `전화번호 (Phone Number)`, `로봇이 아닙니다` 박스에 체크를 한 후 `Send code`를 클릭합니다.
- 전송된 코드를 입력하고 `Verify`를 클릭하면 인증이 완료됩니다.
<br>

### 3. Script 실행하기 (Run 1 script)
- `Course`에서 강의를 진행하거나 직접 `Notebook`을 생성하여 아무 코드나 실행해보면 달성할 수 있습니다.
- `4. Competition에 참가하기`에도 실행하는 과정이 있으니 건너뛰어도 괜찮습니다.
<br>

### 4. Competition에 참가하기 (Make 1 competition or task submission)
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

### 5. 댓글 달고 다른 사람의 게시물이나 댓글에 Upvote 하기 (Make 1 comment & Cast 1 upvote)
- `Discussion`에서 자신이 원하는 Topic에 들어가서 관심있는 글을 클릭합니다. (`Site Forums`의 `Getting Started`에 들어가보는 것을 추천드립니다.)
- 글을 잘 읽어보고 `댓글`을 작성합니다. 글이 유용하거나 마음에 들었다면 `Vote`도 눌러줍시다.
<br>

### 6. Kaggle `Contributor` 되기 완료!

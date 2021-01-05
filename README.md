# Kaggle-Guide

## 목차
1. [Kaggle이란 무엇인가요?](#kaggle이란-무엇인가요)
2. [Kaggle은 어떻게 활용되나요?](#2.kaggle은-어떻게-활용되나요)
3. [Kaggle Competition?](#3.kaggle-competition)
4. [Kaggle 시작하기](#4.kaggle-시작하기)
5. [Contributer 되는 법](#5.contributer-되는-법)
6. [Notebook이란 무엇인가요?](#6.notebook이란-무엇인가요)
7. [Notebook 사용하는 법](#7.notebook-사용하는-법)
8. [Competitions with Notebooks](#8.competitions-with-notebooks)
9. [Competitions 세부 사항](#9.competition-세부-사항)
10. [Competition의 규칙](#10.competition의-규칙)
11. [Competition의 Data](#11.competition의-data)
12. [Competition에 사용된 최신 기술](#12.competition에-사용된-최신-기술)
13. [Kaggle의 Dataset과 API](#13.kaggle의-dataset과-api)
14. [Kaggle에서 자주 사용하는 LightGBM](#14.kaggle에서-자주-사용하는-lightgbm)
15. [Kaggle에서 자주 사용하는 fast.ai](#15.kaggle에서-자주-사용하는-fast.ai)
<br>

***

<br>

# 1.Kaggle이란 무엇인가요?
- __`Kaggle`__ 은 데이터 분석 경진 대회를 주최하는 플랫폼입니다.
- 경진대회는 회사의 `연구 과제, 주요 서비스`를 위해 분석이 필요한 데이터를 제공해서 주최하는게 일반적입니다.
![1](https://user-images.githubusercontent.com/61633137/103594874-3c684d80-4f3d-11eb-9300-c33588266c63.png)
<br>

- __`인공지능, 머신러닝 붐`__ 이 일어나면서 참가자 수가 계속 증가해왔으며 2017년 `구글`의 모회사 __'Alphabet'__ 에 인수되기도 하였습니다.
- Alphabet의 인수 이후 Kaggle은 단순한 플랫폼이 아닌 데이터 사이언티스트, 엔지니어들에게 매우 중요한 사이트가 되었습니다.
<br>

## Kaggler? Kaggling?
- 마치 구글에서 검색하는 것을 __`Googling`__ 이라고 하는 것 처럼 <br>
  Kaggle의 사용자는 __`Kaggler`__, Kaggle에서 활동하거나 Competition에 참가하는 것은 __`Kaggling`__ 이라고 합니다.
<br>

## Competition외 다른 것들
- __Jobs__
  - Jobs를 원래 제공해왔으나 2020년 12월 22일 서비스를 종료했습니다.<br>
    간단하게 요약하자면 이용자 수가 적어서라네요.<br>
    자세한 내용은 https://www.kaggle.com/jobs-board-closed 여기서 읽어보시길 바랍니다.
- __Course__
  ![image](https://user-images.githubusercontent.com/61633137/103596261-e0072d00-4f40-11eb-9e50-2315e734d267.png)
  - `Python`, `머신러닝`, `시각화` 등에 대한 실무, 실용적인 강의들을 제공합니다.
  - 체계적으로 배우지 못했거나 최신 기술이 아닌 강의를 공부했다면 Kaggle의 Course가 꽤 유용할 수 있습니다.
<br>

## Kaggle의 또다른 특징
- __영어__
  - 전 세계의 데이터 사이언티스트들이 모이므로 기본적으로 `영어`를 사용합니다.
  - `Competition의 공지사항`, `데이터 세트(Dataset)`, `토론(Discussion)`도 영어로 이루어집니다. (영어 공부 필수!! 또는 `파파고`..)<br>
    아래는 Discussion과 Site Forum 사진입니다.
  ![image](https://user-images.githubusercontent.com/61633137/103596175-a59d9000-4f40-11eb-9e8c-90fc24e51347.png)
  - 실제로 Competition 입상자들의 프로필을 살펴보면 `미국`, `러시아`, `중국`, `인도`, `한국` 등 다양합니다.
- __프로그래밍 언어__
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
## 데이터 분석을 위한 인프라로 활용
- Kaggle은 `웹 기반`으로 데이터 분석에 필요한 도구를 제공해줍니다.(Notebook)
- 다양한 Kaggler들과 커뮤니티를 이루고 있어 경쟁과 협력이 가능합니다.
<br>

## Notebook
- Kaggle에서 제공하는 __`데이터 분석용 프로그래밍 환경`__입니다.
- SaaS 환경으로 Notebook에 작성한 코드를 서버에서 실행하는 방식입니다.
- 프로그래밍 환경을 제공해주므로 별도의 개발 환경 구축이 필요없습니다.(Python 설치, Anaconda 설치 등등 필요 X)
- __`Jupyter Notebook`__ 을 참고해 만들어져 비슷합니다.
- 기본적으로 `4Core CPU + 16GB RAM`을 제공합니다. `GPU 서버`는 `2Core CPU + GPU + 13GB RAM`을 제공합니다.<br>
  __`사용 횟수 제한없이 무료로 제공`__ 해주며 `GPU는 1주일에 30시간` 동안 사용할 수 있습니다.
<br>

## Dataset 활용하기
![image](https://user-images.githubusercontent.com/61633137/103597920-b18b5100-4f44-11eb-8f02-df689352a762.png)
- 머신러닝 기반의 데이터 분석 프로그램을 개발할 때 가장 먼저 해야하는 것은 __`Dataset`__ 을 준비하는 것입니다.
- 학술 목적으로 공개되었거나 Kaggler가 만들어 공개한 Dataset는 누구나 사용할 수 있습니다.
- 만약 공개하고 싶지 않은 Dataset이라면 __`Private`__ 설정을 통해 외부에는 공개하지 않을 수 있습니다.
- 한 번이라도 Dataset이나 Notebook을 `공개`로 설정하면 `Apache 2.0 License`가 적용되므로 신중하게 결정해야 합니다.
<br>

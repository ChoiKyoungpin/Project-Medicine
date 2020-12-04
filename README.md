# Project-Medicine
<br>
<p align="center"> <img src="https://user-images.githubusercontent.com/68524500/100968395-9bb8f380-3574-11eb-97e9-d32ba2bea425.jpg" width="600px"></p>
<br>
<b>"약 먹는 시간을 놓치거나, 복용하고 있는 약의 정보와 효과를 알고 싶은 사람들을 위한 서비스"</b>
<br><br>

# 목차
1. [프로젝트 목표](#프로젝트-목표)
2. [개발환경](#개발환경)
3. [데이터베이스](#데이터베이스)
4. [핵심기능](#핵심기능)

<br><br>

## 프로젝트 목표

<a name="프로젝트-목표--아날로그-방식-개선-목적"></a>
* [**아날로그 방식 개선 목적 :** ](#프로젝트-목표--아날로그-방식-개선-목적) 식사시간을 기준으로 정하는 아날로그 방식에서 `복용알림 서비스로의 개선 목적.`

<a name="프로젝트-목표--복용-100%-효과-목적"></a>
* [**복용 100% 효과 목적 :**](#프로젝트-목표--복용-100%-효과-목적) 약 동력의 기반하여 `최적의 재 복용 시간`을 알림.

<a name="프로젝트-목표--체내-약효능-시기-인지"></a>
* [**체내 약효능 시기 인지 :**](#프로젝트-목표--체내-약효능-시기-인지) 체내에 약의 효과가 작용하고 있는 것을 `시각적 그래프`로 알려 확인.

<br><br>

## 개발환경

* 언어 
  * JAVA  `EE`  
  * HTML5/CSS3  
  * JavaScript `ES5`
* 프레임 워크  
  * Jqueryv`3.2.2`  
  * node.jsv`12.0`
* 서버(WAS)  
  * Apache Tomcat`v8.0`
* 개발도구  
  * Eclipse-JEE-Mars-2  
  * MySQL WorkBench
* 커뮤니티  
  * Github

<br><br>

## 데이터베이스
<br>
<p align="center"> <img src="https://user-images.githubusercontent.com/68524500/100970654-affeef80-3578-11eb-87ac-e3b478290c47.jpg" width="600px"></p>
<br><br>

## 핵심기능

<a name="핵심기능--약정보-검색"></a>
* [**약정보 검색 :**](#약정보-검색) 복용 중인 약의 기본 정보, 효능, 용법, 주의사항, 부작용 안내
  * OpenAPI 약 5만5천개의 정보와 약 부작용 데이터 100개를 자바코드로 파싱 (사진. OpenAPI. 1,2) 
  * Jquery의 AutoComplete 기능을 이용하여 검색시 자동완성기능 구현 (사진. AutoComplete)
  * 약 이름을 검색하면 효능,용법,주의사항 뿐 아니라 부작용까지 알 수 있도록 구현 (사진. Effect)
 <br> 
 <p align="center"><b>OpenAPI. 1</b><img src="https://user-images.githubusercontent.com/68524500/100977032-ba72b680-3583-11eb-86a1-4f249f9dc233.png" width="600px"></p>

 <b>OpenAPI. 2</b><p align="center"><img src="https://user-images.githubusercontent.com/68524500/100977037-bba3e380-3583-11eb-83ab-89afb2e1151a.png" width="600px"></p>

 <b>AutoComplete</b><p align="center"><img src="https://user-images.githubusercontent.com/68524500/100977830-e0e52180-3584-11eb-9b36-cdfb9845dc87.jpg" width="600px"></p>

 <b>Effect</b><p align="center"><img src="https://user-images.githubusercontent.com/68524500/100979600-56ea8800-3587-11eb-8228-a18d07be6d63.jpg" width="600px"></p>
<br>

-------------------------------------------------------------------------------

<a name="핵심기능--약-복용-그래프"></a>
* [**약 복용 그래프 :**](#약-복용-그래프) 복용 주기에 맞춘 약 효능 그래프
  * 임의로 만든 약 동력 그래프를 시간에 따라 그리게 되고, 복용주기가 끝나면 그래프는 멈추도록 설계함.
  * 약의 효과가 발현하는 40% 지점부터 (임의로 지정) 약 효과가 발현하고 있다는 신호를 주기위해 `gif 이미지를 띄워 표시함.`
 
  <p align="center"><img src="https://user-images.githubusercontent.com/68524500/100954662-5686c880-3558-11eb-9f9b-1108201da02d.gif" width="600px"></p>
<br>

-------------------------------------------------------------------------------

<a name="핵심기능--재복용-문자발송-알림서비스"></a>
* [**재복용 문자발송 알림서비스 :**](#재복용-문자발송-알림서비스) 약 복용 주기를 등록하여 복용 시간에 맞춰 문자 메세지 전송
  * 재복용의 타이밍을 계산하고 적절한 시간에 재복용 알림 문자를 발송하여 재복용을 유도
  <p align="center"><img src="https://user-images.githubusercontent.com/68524500/100954666-571f5f00-3558-11eb-8ee5-f43bb0f55112.jpg"></p>  
<br>

-------------------------------------------------------------------------------

<a name="핵심기능--전국-약국-지도찾기서비스"></a>
* [**전국 약국 지도찾기서비스 :**](#전국-약국-지도찾기서비스) 전국 약국위치를 파악 할 수 있는 지도
  * 약국의 위치를 표시하는 Marker기능과  약국 정보를 나타내는 InfoWindow, 밀집도를 알려주는 클러스터러 기능을 사용
  * Marker가 한 곳에 밀집되어 있을 때, 밀집된 Marker의 수를 표시하기 위해서 Clusterer 기능을 구현함
  <p align="center"><img src="https://user-images.githubusercontent.com/68524500/100988878-8c956e00-3593-11eb-9fdc-1e71f6fec4e7.jpg"></p> 
  
  <p align="center"><img src="https://user-images.githubusercontent.com/68524500/100988880-8dc69b00-3593-11eb-905f-16dd375f6c45.jpg"></p> 
<br>

-------------------------------------------------------------------------------

<a name="핵심기술--실시간-채팅상담"></a>
* [**실시간 채팅상담 :**](#실시간-채팅상담) 관리자와 일반유저의 1대일 채팅
  * Admin으로 접속 했을 때에는 관리자 채팅 표시가 나타나게 하고, 일반 유저일 경우 실시간 상담 로고만 나타나도록 설정함.
  * 관리자 채팅으로 접속 시, 일반 유저들이 작성 한 채팅창이 뜨게 작성하였고 `실시간 채팅`이 가능하도록 구현함. 
  * 일반 유저가 실시간 상담을 종료하면 `관리자 채팅에서의 채팅방도 사라지게 구현함.`
  <p align="center"><b>관리자 실시간 채팅 상담 (실시간 문의 – 고객)</b><img src="https://user-images.githubusercontent.com/68524500/100990746-928c4e80-3595-11eb-9c79-8508a08fd1ad.jpg"></p> 
  
  <p align="center"><b>관리자 실시간 채팅 상담 (실시간 문의 – 관리자)</b><img src="https://user-images.githubusercontent.com/68524500/100990740-915b2180-3595-11eb-8e1c-5f0f62a36703.jpg"></p> 
<br>


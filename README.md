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
  * OpenAPI 약 5만5천개의 정보와 약 부작용 데이터 100개를 자바코드로 파싱  
  * Jquery의 AutoComplete 기능을 이용하여 검색 시자동완성기능 구현
 <br>
 <p align="center">OpenAPI. 1<img src="https://user-images.githubusercontent.com/68524500/100977032-ba72b680-3583-11eb-86a1-4f249f9dc233.png" width="600px"></p>

 <p align="center">OpenAPI. 2<img src="https://user-images.githubusercontent.com/68524500/100977037-bba3e380-3583-11eb-83ab-89afb2e1151a.png" width="600px"></p>

 <p align="center">AutoComplete<img src="https://user-images.githubusercontent.com/68524500/100977830-e0e52180-3584-11eb-9b36-cdfb9845dc87.jpg" width="600px"></p>
<br>
 
 
 
 

<a name="핵심기능--약-복용-그래프"></a>
* [**약 복용 그래프 :**](#약-복용-그래프) 복용 주기에 맞춘 약 효능 그래프
<br>



<a name="핵심기능--재복용-문자발송-알림서비스"></a>
* [**재복용 문자발송 알림서비스 :**](#재복용-문자발송-알림서비스) 약 복용 주기를 등록하여 복용 시간에 맞춰 문자 메세지 전송
<br>



<a name="핵심기능--전국-약국-지도찾기서비스"></a>
* [**전국 약국 지도찾기서비스 :**](#전국-약국-지도찾기서비스) 전국 약국위치를 파악 할 수 있는 지도
<br>



<a name="핵심기술--실시간-채팅상담"></a>
* [**실시간 채팅상담 :**](#실시간-채팅상담) 관리자와 일반유저의 1대일 채팅
<br>


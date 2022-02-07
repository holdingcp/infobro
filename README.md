# infobro


### 구현배경  
- 수도권 내 부동산 서비스가 특정 지역에 집중화되어있다는 문제를 인지함.
- 여러 과정을 거치며 해당 문제는 중개인들이 객관적인 정보를 통하여 중개 지역을 선
택하는 것이 아니라 정보의 부족함으로 인해 해당 지역의 경쟁률, 지역 특성 등을 고려하
지 않고 중개 지역을 선택하여 발생하는 것이라는 걸 발견함.
- 사회적으로 중개 서비스의 낭비가 공공에 발생함.
	→ 위의 사회, 경제적 문제를 해결에 대한 needs를 포착함.
 
☞ 부동산 거래에 대한 서비스 이외의 부동산 중개 사업의 집중화와 정보 부족에 따른 여러 문제점 발생. 고로 중개인들은 본인들의 소득을 극대화하기 위한 needs를 가지고 있음. 이를 충족하기 위해 중개인들이 그들의 사업 소득을 극대화 할 수 있도록 데이터를 가공하여 제공하는 서비스 구현을 통해 사회, 경제적 낭비를 최소화하고자 함.

### 구현목적  
본 서비스의 개발 목적은 부동산 시장에서의 중개 인력의 지역적 불균형을 해결하기 
위함이다. 현재 부동산 시장은 중개인들이 객관적인 데이터를 근거로 사업 영위 지역을 
선택하지 않아 특정 지역에 집중화되어있는 상태이다. 
본 팀은 지역별 중개 수익과 관련된 데이터를 중개인에게 제공함으로써 자연스럽게 중개 
인력이 거래 시장에 적절히 분산되어, 문제가 되고 있는 국내 중개 서비스의 비효율성을 
해결하고자 한다. 이를 통해 중개인들은 그들의 수익 창출에 도움을 줄 수 있는 데이터를 
근거로 수익을 최적화 할 수 있으며, 공공 또한 보다 나은 중개 서비스를 지역별 편차 
없이 영위 할 수 있을 것으로 기대한다.  


#### → 사회적 가치 : 중개서비스 자원이 효율적으로 배분됨에 따라 중개 서비스의 지역 간 불균형 해소에 기여할 수 있음.
#### → 경제적 가치 : 중개인들은 그들의 수익 창출에 도움을 줄 수 있는 데이터를 근거로 수익성 최적화 가능



### 주요기능 
* 중개인의 소득 창출 향상에 도움이 될 관련 데이터 제공
* 지역별 중개인 소득, 중개인 추이, 실거래건수 추이, 부동산 유형(아파트, 단독/다가구, 오피스텔 , 연립다세대, 상업부동산 등)에 따른 중개소득 발생금액 등.
* 멤버십 서비스로는 고도화된 데이터를 기반으로 향후 기대 수익이 상승할 지역을 추천해줄 수 있는 기능을 제공
(지역별 향후 예상소득, 지역별 기대 소득 상승/하강률 예측)


#### 예상 사용자   
중개인으로서 사업 지역을 선택하는데 필요한 데이터를 제공받고 싶은 자


### 개발 일정  
![개발일정](https://user-images.githubusercontent.com/88263745/152727479-9a4cc838-ee24-4b05-88c2-c998692babeb.png)


### 개발 환경  
![개발환경](https://user-images.githubusercontent.com/88263745/152727470-67753445-7e72-409b-b3a1-6f788d7c9583.png)


### 사용 시나리오  
<img src = "https://user-images.githubusercontent.com/88263745/152727453-13994715-e5ae-4274-be34-bc3467c04519.png" width="60%" height="60%">
중개인이 애플리케이션을 이용하는 시나리오이다. 중개인은 가공된 지역별 중개인 수익 관련 데이터를 요청할 수 있다. 서버는 중개인이 요청한 데이터를 데이터베이스에서 검색하여 애플리케이션에 전송한다. 애플리케이션에서는 전달받은 데이터 형태에 따라 API를 이용해 맵, 리스트 형태로 제공한다.


### 시스템 구성도  
<img src = "https://user-images.githubusercontent.com/88263745/152727447-466cf02a-b4f8-4202-a8a8-89258f2cb7ba.png" width="80%" height="80%">


### 서비스 이미지  
<img src = "https://user-images.githubusercontent.com/88263745/152727529-ef60684d-d0a4-49d8-8730-53393d1bdd27.jpg" width="30%" height="30%">

<img src = "https://user-images.githubusercontent.com/88263745/152727539-604543f2-7b72-4b9a-8cfc-1d03de1789d8.jpg" width="30%" height="30%"> <img src = "https://user-images.githubusercontent.com/88263745/152727545-09ec1951-f130-427d-bf1a-c09ad828ee54.jpg" width="30%" height="30%">

<img src = "https://user-images.githubusercontent.com/88263745/152727546-ebf2f0fe-4465-487c-a8a9-80b0a6a1a00d.jpg" width="30%" height="30%"> <img src = "https://user-images.githubusercontent.com/88263745/152728014-b6813fcf-b518-4ec1-92fa-5b8b2a2983f9.jpg" width="30%" height="30%"> <img src = "https://user-images.githubusercontent.com/88263745/152727563-36854a8f-1e6a-4408-9f98-3107c8c6e268.jpg" width="30%" height="30%">

<img src = "https://user-images.githubusercontent.com/88263745/152727570-ff13da1c-e2a4-47e9-8334-6e2aee8aa54f.jpg" width="30%" height="30%"> <img src = "https://user-images.githubusercontent.com/88263745/152727575-565b3d13-eecf-4379-b44e-d39210909b2f.jpg" width="30%" height="30%">

<img src = "https://user-images.githubusercontent.com/88263745/152727579-4eb0103f-6d7e-4de7-a8cc-c96adb9a3635.jpg" width="30%" height="30%">


### 향후 목표  
   본 프로젝트를 통해서 부동산 값 폭등에 비례한 과도한 중개수수료 상승 문제. 그리고 중개인들이 사업지역을 선택할 때 정보의 부족으로 효율적으로 중개지역을 선택하지 못해 발생하는 여러 사회적 비효율성을 해결하기 위해 부동산 매수/매도인들이 수수료의 부담을 조금이라도 덜 수 있는 공동중개 방식을 적극적으로 이용할 수 있도록 하는 앱과 중개인들에게 지역별 중개소득과 관련된 전반적인 정보 및 향후 1년의 기대소득을 제공하는 앱을 개발 및 구현하였다. 해당 앱들을 통하여 중개서비스 자원이 효율적으로 배분됨에 따라 서비스의 지역 간 불균형 해소 및 중개인들의 수익 창출 향상 효과를 기대할 수 있다.  
해당 프로젝트는 long-term 프로젝트로써 서비스를 계속해서 보완해나갈 예정이며, 우선 일반사용자용 앱의 UI를 좀 더 유저친화적으로 업데이트 할 것이고 현재 중개인용 앱에서 제공되고 있는 정보인 지역별 중개인 평균 예상소득, 부동산 실거래 건 수 및 총 매매 금액 외에 중개인들에게 도움이 될 만한 정보들을 계속해서 추가해 나갈 예정이다.

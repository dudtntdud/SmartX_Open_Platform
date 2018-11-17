# KOREN SmartX_Open_Platform

  KOREN SmartX 오픈 플랫폼은 KUF(KOREN 연구협력포럼) 참여 대학교 컨소시엄을 중심으로 2017 ~ 2019년에 걸쳐 진행되는 KOREN SDI 고도화와 연계하면서 2017년부터 단계적으로 구축하고 있는 IoT-Cloud 서비스 대응 KOREN SmartX 오픈플랫폼은  <그림 1>과 제시한 대로 다음과 같은 특징을 가진다.


![Picture1](./images/Picture1.png)

그림 1. 산업인터넷 확살을 위한 KOREN 오픈플랫폼의 단계별 실증


  국내 다수 기관(광주과학기술원, 제주대학교, KOREN NOC, 전남대학교, 건국대학교)에 산재한 IoT-Cloud 대응 SmartX Box(Type O/C/S)들을 KOREN을 통하여 10Gbps 속도로 연결하고 이들을 광주 과학기술원에 위치한 컨트롤타워에서 관제한다. 이를 통해 제공되는 KOREN SmartX Playground(공용개발환경)를 개발자들이 자유롭게 활용하면서, 분산된 드론과 스마트폰 등을 통하여 수집한 센서 및 동영상 데이터를 모아서 시각화를 제공하는 [Smart Air IoT-Cloud 서비스](https://github.com/KOREN-Platform/IoT-Cloud_Services/tree/master/Smart_Air_IoT_Cloud_Service)를 포함한 다양한 IoT-Cloud 서비스들을 마이크로서비스 구조의 컨테이너 기반으로 오픈소스 기반의 KOREN SmartX OpenPlatform을 활용하여 손쉽게 실증하는것이 가능하다.

## System Architecture
  * Main Architecture
![Architecture](./images/Architecture.png)
  * Network Architecture
![Boxes](./images/Boxes.png)

### Component Links
  
  * Service
     - [IoT-Cloud Application Services Workflow](https://github.com/KOREN-Platform/IoT-Cloud_Services/tree/master/IoT_Cloud_Service_Workflow)
     - [Smart Air IoT-Cloud Service](https://github.com/KOREN-Platform/IoT-Cloud_Services/tree/master/Smart_Air_IoT_Cloud_Service)
     - [Service Visualization & IoT data analysis tool](https://github.com/KOREN-Platform/IoT-Cloud_Services/tree/master/Service_Visualization_Analysis_Tool)
  
  * Control Tower
     - O+P Center
     - S Center
     - V Center

  * Boxes
    - [O-Box](https://github.com/KOREN-Platform/SmartX_Playground/blob/master/Playground_Introduction_Guide/User_Guide/Type-O%20%EB%82%B4%EB%B6%80%20%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC%20%EC%84%A4%EC%A0%95%20%EB%B0%8F%20%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8%20%EC%84%B8%EB%B6%80%20%EC%84%A4%EB%AA%85.pdf)
 : IoT와 Cloud 사이에 위치하여 유연한 연결성을 제공하는 SD-Access의 적용을 위한 Box. Type O SD-Access Box는 와이파이 및 유선 연결을 통해 드론, 스마트폰과 같은 IoT 기기들에게 네트워킹을 제공하며, 관제타워의 SD-Access SDN 제어기의 제어 하에 IoT 어플리케이션이 생성하는 데이터를 클라우드로 전달하는 역할을 한다.
    - C-Box(클라우드 대응)
    - S-Box
 : ONOS SDN 제어기를 기반으로 Server와 Switch 파트를 한 하드웨어에 담고 있는 형태의 융합형 자원 Box


### Links
  - [Playground User Guide](https://github.com/KOREN-Platform/SmartX_Playground/blob/master/Playground_Introduction_Guide/User_Guide/readme.md)
  - [상세가이드](https://goo.gl/xyXfpd)
  - [Collaboration_2017](https://github.com/KOREN-Platform/Collaboration_2017)
  - [Technical_Documents](https://github.com/KOREN-Platform/Technical_Documents)
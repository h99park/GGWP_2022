# Intro

게이머들은 기존에 같이 게임할 사람을 개인이 사용하는 커뮤니티에서 구인하거나, 각 게임별로 나뉘어 있는 플랫폼을 주로 사용해왔다. 대부분 유저 모집만을 위한 서비스는 없었기 때문에 모집에 있어서 소통방법, 유저 검증 등의 어려움이 존재했다. 따라서 '종합 게임 유저 모집 서비스- <GGWP: Good Gamers Well Paried>'를 제공하여 불편함을 해소하고자 한다.
![image](https://user-images.githubusercontent.com/105280709/206725823-8901dbaa-f0c0-4869-90db-13b336c74ddf.png)
  

본 프로젝트는 함께 게임할 유저를 모집하는 것에 초점을 맞춰 서비스를 제공하고자 한다. 여러가지의 조건 설정을 통해 다양한 모집 수요를 충족시키고자 한다.  

흔히 게이머들은 음성 및 채팅 채널을 이용할 수 있는 디스코드를 쓰지만, 많은 사람들이 사용하는 대형 디스코드 서버 내에서는 사용자의 신원이 확보되지 않고, 금전거래로 인한 사기나 성희롱과 같은 사례도 빈번하게 일어나곤 한다.  
  
따라서 이번 프로젝트에서는 신원이 보장된 인원과 대화를 나누고 기록된 채팅을 기반으로 신고를 받아 유저를 관리하여 게이머들이 안심하고 사용할 수 있는 서비스를 제공하고자 한다.  
 
Django의 channels 라이브러리를 통해 해당 채팅 기능을 구현하고자 한다.  

# About
![img1 daumcdn](https://user-images.githubusercontent.com/105280709/206723484-aa16adac-d2e2-4e57-9895-03c5f41348ee.png)
Channels는 Django의 네이티브 ASGI(Asynchronous Server Gateway Interface) 지원을 기반으로 구축된다. 웹소켓, 채팅 프로토콜, IoT 프로토콜 등을 처리할 수 있도록 확장을 용이하게 해 준다.  

# Setup
Ubuntu 개발 환경에서 진행됩니다. WSL을 사용하여 Windows에 Linux 설치를 먼저 해주세요.  
(https://user-images.githubusercontent.com/105280709/206724300-e1ef9360-2c8a-4d3e-bca9-479d4896de47.jpg)
Django와 Channels, 그리고 Daphne를 설치해야 합니다. Python 3.8 이상의 버전을 사용해주세요. Daphne는 요구하는 최신버전으로 설치해주세요.  
  
해당 코드는 로컬서버에서 진행되는 것을 전제로 했기 때문에 도커와 Redis server는 사용하지 않은 버전입니다.  

# Usage
manage.py 파일이 존재하는 디렉토리에서 아래 명령을 실행시킵니다.  

python3 manage.py runserver

로컬 서버 주소(http://127.0.0.1:8000/chat/) 를 통해 채팅방의 이름을 입력하고 채팅방에 입장할 수 있습니다.  

# Result

https://user-images.githubusercontent.com/105280709/206725366-7ce878c9-e403-4c57-a2e9-bf6b06a0feba.mp4



# Reference
https://channels.readthedocs.io/en/stable/index.html

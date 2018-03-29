# [2018.03.31] Azure App Service 및 Serverless 핸즈온랩 워크샵

Azure App Service 및 Serverless 핸즈온랩 워크샵 참석자를 위한 사전 준비 리스트입니다.

URL : https://onoffmix.com/event/131652

## HOL(Hands-on Lab) 진행 순서
- 13:00 ~ 13:20 / 사전 설치 프로그램 확인 및 리소스 준비 (20분) - 상훈
- 13:20 ~ 13:40 / App Service 소개 (20분) - 용준이형
- 13:40 ~ 14:10 / 실습1 App Service 생성 및 개발 실습 (30분) - 용준이형
- 14:10 ~ 14:20 / Break Time (10분)
- 14:20 ~ 15:00 / 실습2 간단한 ASP.NET web App 구축 및 배포(Visual Studio 사용) (40분) - 상훈
- 15:00 ~ 15:10 / Break Time (10분)
- 15:10 ~ 15:50 / 실습3 온라인 Azure Functions 개발 실습 (40분) - 태영이형
- 15:50 ~ 16:30 / 실습4 Azure CLI를 이용한 Function 개발 실습 (40분) - 태영이형
- 16:30 ~ 16:40 / Break Time (10분)
- 16:40 ~ 17:20 / 실습5 이미지 프로세싱 실습 (40분) - 태영이형
- 17:20 ~ 18:00 / 실습6 Logic 앱을 사용한 워크플로우 실습 (40분) - 태영이형

## 사전 설치 프로그램 

#### 강좌 참여 시 사전 준비 및 설치 사항(필수)
- Visual Studio Code 설치 : https://code.visualstudio.com/ 
- Azure CLI 설치
    - Windows : https://aka.ms/InstallAzureCliWindows 
    - Mac OS : https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest 
- Postman 설치 
    - https://www.getpostman.com/postman 
- Azure Storage Explorer 설치 
    - https://azure.microsoft.com/en-us/features/storage-explorer/ 

#### 다음은 순서대로 설치하시기 바랍니다 
- Node 8.5 이상의 Stable 버전 설치 (9.X 버전은 안됩니다) 
    - https://nodejs.org/en/ 
- .NET Core 2.0 SDK 설치
    - https://www.microsoft.com/net/download/windows    
- Azure Functions Core Tools 설치 (CMD 명령 프롬프트에서 실행) 
    - npm i -g azure-functions-core-tools@core     
    - Mac OS인 경우 : sudo npm i -g azure-functions-core-tools@core --unsafe-perm 
- Azure Functions Pack 설치 (CMD 명령 프롬프트에서 실행) 
    - npm i -g azure-functions-pack 

## Azure Portal 설정

#### 리소스 그룹 생성   
- 이름 : rg-aspkr-bootcamp   
- 위치 : Southeast Asia  

#### As plan 생성  
- 이름 : aspkr-BootCamp-Dev-Plan  
- 가격 : S1  
- 위치 : Southeast Asia   

#### 저장소 계정 생성   
- 이름 : aspkrholstor<전화번호 뒷자리4>  
- 위치 : Southeast Asia  
- Replication : LRS   

#### Web App 생성   
- 이름 : aspkr-hol1-<전화번호 뒷자리4>, (실습 1)
    - AS-Plan : aspkr-BootCamp-Dev-Plan 선택 
- 이름 : aspkr-hol2-<전화번호 뒷자리4>, (실습 2)
    - AS-Plan : aspkr-BootCamp-Dev-Plan 선택  

#### Function App 생성   
- 이름 : aspkrFunc1-<전화번호 뒷자리4>, 일반 실습용  
    - AS-Plan : aspkr-BootCamp-Dev-Plan 선택  
- 이름 : aspkrFunc2-<전화번호 뒷자리4>, CLI 실습용  

#### Face API 생성  
- 이름 : aspkr-FaceApi  
- 위치 : WestUS  
- 가격 : F0 혹은 S0  

#### Logic App  
- 이름 : FB-TTS-MAIL 

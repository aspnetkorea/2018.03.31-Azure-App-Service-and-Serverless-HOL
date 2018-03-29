# [2018.03.31] Azure App Service 및 Serverless 핸즈온랩 워크샵

Azure App Service 및 Serverless 핸즈온랩 워크샵 참석자를 위한 사전 준비 리스트입니다.

URL : https://onoffmix.com/event/131652

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

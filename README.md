Nodejs + express + handlebars + bootstrap
======================

# 1. 서버 구성  
## 1.1. AWS Lightsail 서비스 이용 
- Lightsail(https://lightsail.aws.amazon.com) AWS 매니저에서 링크로 이동
- Create an instance(서버 인스턴스 생성) --> Node.js(7.10.0) 생성
- Create a static IP address(IP 활당) -->13.115.40.134 계정 : bitnami
- Account SSH Keys Pairs 설정--> 로컬에 key 다운로드(LightsailDefaultPrivateKey-ap-northeast-1.pem) 
- Networking Firewall 설정 -->  TCP : 3000 추가

## 1.2. 서버 접속 Client
### 1.2.1. Xshell5 사용 
	1. pageant 를 사용하여 pem 파일을 ppk 파일로 변환(EditPlus 사용을 위해)
	2. Xshell5으로 public key 로그인 
![shell 접속](http://13.115.40.134/img/shell.PNG)

****
# 2. Express + Handlebars 

## 2.1. Express 설치 

	1. $ npm install express
	2. $ express ExpressDevTest(기본적으로 jade 로 설치됨)
	3. public, routes, views 폴더가 생성되고 package.json, app.js가 생성됨을 확인할 수 있다.
        4. Package.json에 보면 Dependencies에 express와 jade, body-parser, cookie-parser, debug, morgan, 
	   Serve-favicon이 등록되어 있는데 express를 제외한 나머지 모듈은 npm install으로 추가 module 설치 
	   반드시 프로젝트 디렉토리 내에서 설치 실행
           $ npm install


   

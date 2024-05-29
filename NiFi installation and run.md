NiFi 설치 및 구동 (Win 11)

1. 준비물
   - NiFi : https://nifi.apache.org/download/
     
     ![1](https://github.com/vmflsfldk/NiFi/assets/25484514/d14eb66d-a126-4eb2-86a4-2f850fc82276)
   - Java : NiFi 2.0.0 - M3 기준) JDK version 22 이상 필요 / https://www.oracle.com/kr/java/technologies/downloads/
     
     ![2](https://github.com/vmflsfldk/NiFi/assets/25484514/37d245aa-9381-49b7-a913-498568857ce8)
2. Java 환경 변수 설정
   - 시스템 속성 - 고급 - 환경 변수 - 시스템 변수 - 새로 만들기
   - 변수 : CLASSPATH / 값 : %JAVA_HOME%lib 생성
   - 변수 : JAVA_HOME / 값 : JDK설치 경로 (default : C:\Program Files\Java\jdk-22) 생성
     Path 변수에
   - C:\Program Files\Common Files\Oracle\Java\javapath
   - %JAVA_HOME%bin
   - C:\Program Files (x86)\Common Files\Oracle\Java\javapath 추가
     
     ![3](https://github.com/vmflsfldk/NiFi/assets/25484514/c0789483-23f1-4cd9-ab68-c3e5008f8c0d)

3. 다운로드 받은 NiFi 압축해제
   - 폴더 경로에 한글포함되는 경우는 비추천


   ![4](https://github.com/vmflsfldk/NiFi/assets/25484514/6b67246e-175e-491b-ac63-47e37f311a5d)

4. NiFi Run
   - NiFi 폴더 내 bin - run-nifi.bat 실행

   ![5](https://github.com/vmflsfldk/NiFi/assets/25484514/8716e21a-ea35-4430-9357-b2d8957e0e75)

   위와 같이 문구가 출력되면 정상 구동 중

5. NiFi 접속
   - 별도 설정 하지 않을 시, 기본 접속 URL : https://localhost:8443/nifi
  
   ![6](https://github.com/vmflsfldk/NiFi/assets/25484514/be38a0fe-b2f5-4147-b15c-7dbd9d7a94c6)

   Nifi - logs - nifi-app.log 파일에서 확인 가능

   ID 및 PassWord 는 별도 설정 하지 않을 시, 자동 생성 되어 nifi-app.log에서 확인 가능

   ![7](https://github.com/vmflsfldk/NiFi/assets/25484514/7983a4de-7a14-4588-a98e-d7fa9b821a8e)

   ID 및 PassWord 는 별도 설정은 conf - login-identity-providers.xml 에서 설정 가능

   ![8](https://github.com/vmflsfldk/NiFi/assets/25484514/3cf3b2bf-4b4b-4c41-aa07-bd07b29080e5)

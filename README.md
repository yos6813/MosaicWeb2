1. Spring Starter Project 생성

	- Name : MosaicWeb
	- Type : Gradle(BuildShip)
	- Packaging : war
	- Group : com.hybrid
	- Artifact : MosaicWeb
	- Package : com.hybrid
	
	- Dependencies 선택 : web

2. 형상관리 
	
	- Remote Repository 생성(github.com)
	- Local Repository 생성
		* git status //깃 상태 확인
		* git log //깃 기록 확인
		* dir /A > .gitignore
		* notepad .gitignore
		* git init
		* git add . / git add *
		* git commit -m "first commit"
		 
	- Local --> Remote push(최초 동기화)
		* git remote add origin >> https://github.com/yos6813/MosaicWeb.git
		* git remote -v //깃 경로 확인
		* git remote remove //깃 경로 제거
		* git push -u origin master
		 
	- 개발자 2가 clone 수행
		* git clone https://github.com/yos6813/MosaicWeb.git
		* git clone https://github.com/yos6813/MosaicWeb.git MosaicWebDev //폴더 지정
		* Eclipse Gradle Import
		
3. HTML 설정

	- 설정 불필요
	- mkdir src/main/webapp 폴더 생성
	- notepad src/main/webapp/Hello.html
	- gradle bootrun
	- Web Browser -> http://localhost:8080/Hello.html
	
4. JSP 설정
	
	- mvnrepository.com -> search : jasper
	- build.gradle -> dependencies : providedRuntime group: 'org.apache.tomcat.embed', name: 'tomcat-embed-jasper', version: '8.5.4' -> Eclipse 	Gradle 	Refresh
	- notepad src/main/webapp/Hello.jsp
	- gradle bootrun
	- Web Browser -> http://localhost:8080/Hello.jsp
	
5. Servlet 설정
	
	- Properties -> project facets -> Dynamic Web Module 3.1, java 1.8, javascript 1.0 추가
	- MosaicWebApplication.java -> @ServletComponentScan 추가
	- com.hybrid.servlet.HelloServlet.java 생성
	- gradle bootrun
	- Web Browser -> http://localhost:8080/HelloServlet


6. SpringLoaded 설정(리로드 기능)
	
	- mvnrepository.com -> search : springloaded 1.2.6버전
	- build.gradle에 설정(두 곳) 
	  	* 두번째 dependencies -> compile group: 'org.springframework', name: 'springloaded', version: '1.2.6.RELEASE'
	  	* 첫번째 dependencies -> classpath("org.springframework:springloaded:1.2.6.RELEASE")
	- Eclipse Output Directory 변경
	  	* bin -> build/classes/main
	
	
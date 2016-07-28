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
	
	
1. Spring Starter Project ����

	- Name : MosaicWeb
	- Type : Gradle(BuildShip)
	- Packaging : war
	- Group : com.hybrid
	- Artifact : MosaicWeb
	- Package : com.hybrid
	
	- Dependencies ���� : web

2. ������� 
	
	- Remote Repository ����(github.com)
	- Local Repository ����
		* git status //�� ���� Ȯ��
		* git log //�� ��� Ȯ��
		* dir /A > .gitignore
		* notepad .gitignore
		* git init
		* git add . / git add *
		* git commit -m "first commit"
		 
	- Local --> Remote push(���� ����ȭ)
		* git remote add origin >> https://github.com/yos6813/MosaicWeb.git
		* git remote -v //�� ��� Ȯ��
		* git remote remove //�� ��� ����
		* git push -u origin master
		 
	- ������ 2�� clone ����
		* git clone https://github.com/yos6813/MosaicWeb.git
		* git clone https://github.com/yos6813/MosaicWeb.git MosaicWebDev //���� ����
		* Eclipse Gradle Import
		
3. HTML ����

	- ���� ���ʿ�
	- mkdir src/main/webapp ���� ����
	- notepad src/main/webapp/Hello.html
	- gradle bootrun
	- Web Browser -> http://localhost:8080/Hello.html
	
4. JSP ����
	
	- mvnrepository.com -> search : jasper
	- build.gradle -> dependencies : providedRuntime group: 'org.apache.tomcat.embed', name: 'tomcat-embed-jasper', version: '8.5.4' -> Eclipse 	Gradle 	Refresh
	- notepad src/main/webapp/Hello.jsp
	- gradle bootrun
	- Web Browser -> http://localhost:8080/Hello.jsp
	
5. Servlet ����
	
	- Properties -> project facets -> Dynamic Web Module 3.1, java 1.8, javascript 1.0 �߰�
	- MosaicWebApplication.java -> @ServletComponentScan �߰�
	- com.hybrid.servlet.HelloServlet.java ����
	- gradle bootrun
	- Web Browser -> http://localhost:8080/HelloServlet


6. SpringLoaded ����(���ε� ���)
	
	- mvnrepository.com -> search : springloaded 1.2.6����
	- build.gradle�� ����(�� ��) 
	  	* �ι�° dependencies -> compile group: 'org.springframework', name: 'springloaded', version: '1.2.6.RELEASE'
	  	* ù��° dependencies -> classpath("org.springframework:springloaded:1.2.6.RELEASE")
	- Eclipse Output Directory ����
	  	* bin -> build/classes/main
	
	
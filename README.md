서버 계정 추가 부터 서버 환경 셋팅 가이드

root 접속 

>> 사용자 추가
$ useradd 계정명 -m -s /bin/bash

-m : 옵션을 명시하면 홈 디렉토리 생성
-s /bin/bash : 옵션을 명시하면 쉘 환경 설정

>> 패스워드 설정
$ passwd 계정명
비번설정/재설정

>> java가 루트 계정에 설치 되어있을 경우 /etc/profile 에 패스 설정
>> 추가된 사용자가 사용할 경우, 사용자 폴더에 .bashrc 파일이나 .bash_profile에 패스 설정 한다.
>> 확인 java, javac, java -version

>> tomcat 설치

$ wget http://apache.mirror.cdnetworks.com/tomcat/tomcat-8/v8.5.15/bin/apache-tomcat-

8.5.15.tar.gz

>> tomcat 압축 풀기

$ tar -zxvf 파일.tar.gz

>> tomcat 심볼릭 링크

$ ln -s apache-tomcat-.... tomcat


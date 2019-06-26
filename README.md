# Django Tutorial
이 프로젝트는 Django Tutorial을 따라하면서 구현한 Repository입니다.  
프로젝트의 원할한 진행을 위하여 git으로 버전 트래킹을 하진 않았습니다.     
단, Tutorial의 진행 방향 그대로 진행하였으므로 Tutorial을 참고하면 됩니다.  


## Related Links
Official Tutorial : [바로가기](https://docs.djangoproject.com/en/2.2/intro/)   
Blog : [Daim's blog 바로 가기](https://daimhada.tistory.com/186)   


## Environment
개발 환경은 다음과 같습니다.   
#### framework & library
Python : 3.6.5  
Django : 2.2.2  
MySQL : 5.6  
virtualenv :  16.0.0

## Start
다음의 방법으로 Django 환경을 세팅합니다.  
virtualenv를 설치하는 방법은 [링크](https://daimhada.tistory.com/118)를 참고하세요.  

```
# 가상 환경 세팅
 virtualenv venv
 
# 가상 환경 활성화
source venv/bin/activate

# Django 설치
pip3 install Django

# 설치 환경에 따라서 다음과 같이 디렉토리 조정이 필요할 수도 있습니다. 
mysite/
    manage.py
    mysite/
        __init__.py
        settings.py
        urls.py
        wsgi.py
```
Django의 기본 DB는 SQLite이므로 mysql을 사용할 수 있도록 설치합니다.
mysql 설치는 다음의 [링크](https://daimhada.tistory.com/121)를 참고하시면 됩니다.
혹은 아래에 brew 패키지 관리자를 이용해 설치하는 방법으로도 사용 가능합니다.
```
# mysql 설치하기
brew install mysql

# mysql 접속 (password 방식으로 사용자 접속)
mysql -u root -p

# mysql에서 DATABASE 생성
CREATE DATABASE <dbname> CHARACTER SET utf8;

# Django mysql driver 설치
pip3 install mysqlclient

``` 

이 외에 사항들을 위에 관련 링크에 적혀있는 제 블로그 혹은 공식 문서의 튜토리얼을 참고하세요.
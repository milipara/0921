1. 서버 만들 폴더 생성
  mkdir [폴더이름]
2. 가상환경 만들기
python -m venv [가상환경 이름]
3. 가상환경 활성화
source venv/Scripts/activate
4. 가상환경 비활성화
  deactivate
5. 장고 설치

  	pip install django==3.2.13

6. 장고 어드민 설치

  django-admin startproject [프로젝트 이름]  [설치 경로] (설치 경로는 '.'(점)으로 해결)

7. 서버 활성화

     python manage.py runserver

8. 서버 끄기

Ctrl + C



번외

```You have 18 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, contenttypes, sessions.Run 'python manage.py migrate' to apply them.```

오류 발생시

```python manage.py makemigrations```

```python manage.py migrate```

원인 : models 개체에 DB scheme이 반영 안되어서 생긴 문제.
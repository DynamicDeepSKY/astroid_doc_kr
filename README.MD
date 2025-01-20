# 튜토리얼은 아래것이 잘되어 있음
https://techwritingmatters.com/documenting-with-sphinx-tutorial-part-2-implementation



# 시작



# 필요 패키지 인스톨

```
sudo apt-get install python3-sphinx
pip install sphinx_rtd_theme
```

# 테마 바꾸기
gedit conf.py

아래라인 수정

html_theme='sphinx_rtd_theme'

# 컴파일 하기

make html
폴더 들어가서 오프라인으로 확인 가능

# 깃에 업로드

공개로 설정

해당 깃을 아래의 사이트에 연결 하고 퍼블리쉬 하면 됨

https://readthedocs.org/
캐시가 있어서 문서를 업데이트해도 컴파일 시 결과 업데이트가 바로바로 안된다. 그럴 경우 한참 기다렸다 할것
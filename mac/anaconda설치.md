
**Mac에 Anaconda 설치하기**  
anaconda install + jupyter notebook 실행하기

~~~
* os : mac
* prerequiste : homebrew 설치하기
~~~

---

brew는 설치되어 있다고 가정하기.  
먼저 brew를 업데이트해준다.   
~~~
brew update --auto-update
~~~


업데이트 끝나면 brew 커맨드로 아나콘다 설치하기
~~~
brew install --cask anaconda
~~~

설치 끝나면 다음과 같이 나옴.

![스크린샷 2024-03-19 오후 1 02 17](https://github.com/hannie0615/basic_commands/assets/50253860/b8507df7-9b24-4891-af66-85305c814c5e)

설치 끝났으니 이제 세부 설정.  
설치하다보면 터미널에 prefix 경로가 나오는데 path에 설정해주기
~~~
export PATH="/usr/local/anaconda3"
~~~

jupyter notebbok 실행하기 
~~~
jupyter notebook
~~~

![image](https://github.com/hannie0615/basic_commands/assets/50253860/d2841ff5-d9bc-45f1-8310-d1981fcf28bb)
- 끝



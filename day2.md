# git 명령어 복습
## git push 한눈에 보기
![깃 명령어 한눈에 보기](./git%20%EB%AA%85%EB%A0%B9%EC%96%B4%20%ED%95%9C%EB%88%88%EC%97%90%20%EB%B3%B4%EA%B8%B0.png)

## clone
 1. `git clone 저장소 주소`
    - 이렇게 하면 clone 된 폴더가 새로 생긴다 
 2. git pull origin master (origin master 생략가능, origin 이라는 저장소의 master 브랜치의 내용을 가져온다)
 3. Example
```
# TIL-home

$ git init
$ touch day1.md
$ git add .
$ git commit -m "집에서 Day1 작성"
$ git remote add origin https://github.com/edukyle/TIL-remote.git
$ git push origin master
```  

- TIL-home 로컬 저장소의 내용이 TIL-remote 원격 저장소에 그대로 반영됨

- 다른컴퓨터로갔을떄

> 여러분은 이제 강의장에 왔습니다. 강의장 컴퓨터에는 여러분의 TIL 폴더가 없습니다.

```bash
# TIL-class

$ git clone https://github.com/edukyle/TIL-remote.git TIL-class
```


## 끝말잇기
1. 조장은 repository 를 파고 초대를 한다
```bash 
$touch README.md
$git add .
$git commit -m "조장"
$git remote add origin https://github.com/p098765/wordrelay.git
```
2. 조원 turn
```bash
$git clone https://github.com/p098765/wordrelay.git
$git pull origin master
#편집
$git add .
$git commit -m "조원1"
$git push origin master
```
![끝말잇기예제](./%EB%81%9D%EB%A7%90%EC%9E%87%EA%B8%B0%20%EC%98%88%EC%A0%9C.png)

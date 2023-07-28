## git
### git 사용법
#### 프로젝트 폴더 - git
> ```git init``` : 현재 디렉토리에 작업을 진행하겠다, 버전관리 하겠다.
 ```vim 파일명``` : 파일 안에 무엇을 입력함
 ```cat 파일명``` : 파일 내용 확인
 ```ls -al``` : 파일 목록 창
 ```git status``` : 저장소 상태 창
 ```git add 파일``` : 버전 관리 시작 명령어 (추적되기 전, 추적 후 수정때도 사용해야함)
 ```i``` : 입력 가능한 상태로 만들기
 ```1 + esc``` : 입력가능한 창 나가기
 ```w``` :  저장한다
 ```q``` :  나가기 (insert 상태에서 wq입력시 저장 후 나가짐)
 ```git config --global user.name 이름``` : 버전에 이름 새기기
 ```git config --global user.email 이메일``` : 버전에 이메일 새기기
 ```git commit``` : 어떤 내용을 담고있는지의 메시지
 ```git commit -m "커밋 메시지"``` : 커밋 메시지 바로 작성 가능
 ```git log``` :  버전 정보 창(역사, 현재브렌치의 정보)

#### branch
> ```git branch``` : 사용하는 브렌치 알려줌
 ```git branch 브렌치이름``` : 브렌치 생성
 ```git checkout 브렌치이름``` : 브렌치 이름의 브렌치로 들어가짐(전의 브렌치에서 체크아웃됨)
 ```git log --branches --decorate``` : 브렌치 정보를 잘 보여줌
 ```git log --branches --decorate --graph``` : 브렌치 그래프 보여줌
 ```git log --branches --decorate --oneline``` : 한줄로 보여줌
 ```git log master..exp```(브렌치 예시 master-exp) : 브렌치 간의 차이점 확인(master 브렌치에는 없고 exp브렌치에는 있는것 보여줌)

> ##### 병합 merge
 ```git merge exp``` : exp를 master로 merge하라는 명령어 (exp를 master로 병합할 시 1.master로 체크아웃 2.master에서 merge 명령 필요)
 ```git branch -d exp``` : exp브렌치 삭제

### 협업 전략
#### 1. GitFlow
> 브랜치 5개
> - main : 기존 코드 저장
  - develop : 신규 코드 저장
  - feature : 여기서 개발해본 후 안전하게 develop에 merge
  - release : main push 전 임시 브랜치
  - hotfix : 마무리 후 오류 발생 시 main에서 브랜치 하나 빼서 수정 후 push

#### 2. Trunk-based
> 브랜치 하나만 잘 관리하자
> main 하나만 관리, but test 많이 해야함


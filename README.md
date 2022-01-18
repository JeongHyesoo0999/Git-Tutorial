# Git-Tutorial
[Youtube]Dongbinna

#### 1강 Git 설치 및 사용법 익히기
- git : git 사용법 
- git --version : git 버전


##### 연결하기
- git config --global user.name [닉네임]
- git config --global user.email [이메일주소]
- cd C:\Education
- git clone https://github.com/SGongD/Git-Tutorial.git // 다운로드

##### 깃허브에 올리기
- .txt파일 생성
- cd Git-Tutorial
- git add hello.txt(.)
- git commit -m "Add Text File [document.txt]"
- git push

#### 2강 오픈소스의 개요 및 오픈소스 활동을 하는 이유
- contribution활동을 하는 이유 : 구직을 할 때 기록으로 남기 때문에 이력으로 남아서.
- Committer : 실제로 반영을 시킬지 안시킬지 권한을 가지고 있는 사람.

#### 3강 Git이 등장한 배경과 Git의 장점
- 분산적인(합치기, Merge가능) 개발, 효율적인 개발, 비선형적인 개발(branch), 변경 이력 보장

#### 4강 Git의 동작 원리
git add > git commit > git push (<=> git pull)

#### 5강 소스코드 수정하여 Git 저장소에 반영하기
- 해당 프로젝트에 소속된 사람이 아닌 경우(Pull Request)
- 해당 프로젝트에 소속된 사람인 경우
  - 내 컴퓨터에 폴더 만들기 (cd C:\파일명)
  - 클론 진행하기 (git clone URL주소)
  - 다운받은 폴더로 이동(cd Git-Tutorial)
  - 내가 추가/수정하고 싶은 파일 작성
  - 파일의 상태 확인(git status) 
  - 파일 추가(git add 파일명) <-> 만약 내리고 싶다면(git reset 파일명)
  - 복구를 위해 commit 명령어 사용 (git commit -m "Add 파일명 [사유]) 
  - => 커밋 명령어를 잘못 썼다면 (git commit --amend)
  - 만약 깃에 추가하려는 내용을 무시하고 싶다 (git checkout -- 파일명) => 띄어쓰기 주의

#### 6강 Git에서 커밋 내역 수정하기
- 특정한 프로젝트가 언제 파일을 수정했는지
- git pull > 정확히 일치하는지
- 시점으로 돌아가기 (git reset --hard 코드값)
- 만약 특정 시점으로 돌아간 후에 Github도 똑같이 반영하고 싶다면? (git push -f)

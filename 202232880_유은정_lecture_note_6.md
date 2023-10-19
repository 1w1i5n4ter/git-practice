# ✨Open Source SW✨
##  Lecture 6 - _Git_
: Git 사용방법
- 버전 컨트롤할때(for development, other document works) 필수적으로 사용. 
**버전 컨트롤** : 시간이 지남에 따라서 기록하는 거 _ 특정 버전으로 돌아갈 수 있음.
                   
### change  vs snapshots  
change:쌓인 변화들 축적, 각기 버전에서 그 시점에 base에 change를 축적
snapshots: `git에서 사용` 변화를 기록하는게 아니라, 버전2 에서의 스냅샷. 파일 전체를 기록함. 

### local, centralized, and Distributed Version Control
local: <장점> 개인컴퓨터 안에서만 version control 가능. 
       <단점> 다른 사람들과의 협업 어려움.  

centralized: <장점> `협업할때 이게 좋음` + 중앙 서버있음. (중앙 서버에게 요청) 
<단점> 중앙서버에 옮길때 문제 발생

Distributed Version Control:`협업할때 이게 좋음` _ `Git은 여기에 해당` 
:각각의 로컬 컴퓨터가 복사본을 가지고 있음 =서버가 녹다운 되어도 각각의 로컬 컴퓨터에 중앙데이터의 복사본이 있기때문에 중앙서버를 복구할때 사용/반영 + 협업할때 편리.



## Three staed in Git
|  | |
| ------- | ------ |
| Modified | `working directory`:staging area로 먼저 옮기기.  |
| Staged  | `staged Area` 커밋단계를 위한 준비단계.  이부분을 staging area에 가서 대기 |
| Committed | `git directory` repository에 (특정 시점의 version) 저장 |

### Git config: first-time setup
 [`definition from chat gpt`](https://chat.openai.com/share/09db1466-772a-4be4-9888-893546d2b579)
 
shell 명령어에서 파일을 지우는 거 > rm
git rm --cashed : 파일시스템에서 사라지는 게 아니라 git(staginga area)에서 사라지는거임

###### +공부하면서 생긴 질문은 Q&A 게시판에!
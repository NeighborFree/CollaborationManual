# CollaborationManual 

### NeighborFree team Git Branching Strategy 
  *NeighborFree 팀 협업을 위한 git branch 전략*


## :octocat: Git flow branching Strategy

branch | 역할
---- | ---- 
master | 배포를 위한 가장 최신의 release version 코어 브랜치 
develop | 개발 완료 상태인 브랜치로 feature branch들을 merge하기 위한 코어 브랜치
features | 개발을 위한 모듈 별 브랜치
hotfix | 배포된 버전 버그 수정을 위한 브랜치
release | 배포 버전에 대한 fix 후 배포 준비 브랜치



>* master, develop 브랜치의 경우 코어 브랜치이므로 삭제 및 수정으로 인해 해당 Repository에 큰 영향을 끼치므로 Repository 오너에게만 권한을 부여한다.
>* 개발은 features - develop - release - master 순서로 merge 진행한다.
>* hotfix 브랜치는 배포 후 따로 사용 분업하여 담당중이 아닌 기능 개발에도 다른 팀원들이 확인 후 bug fix를 할 수 있다.


## :name_badge: Git branch naming
 
* 핵심이 되는 master, develop의 경우 본래 이름대로 사용한다.

* features : feature/기능 형식으로 한다. 
  * **EX) feature/signup**

* features : issue 발생 후 수정을 할 경우 feature{issue-number}-{feature-name} 형식을 사용한다. 
  * **EX) feature/443-signup , signup과 관련된 443번 issue가 해결을 위한 branch**

* release : release- 의 형식을 사용한다. 
  * **EX) release-0.1**


* hotfix : hotfix- 의 형식을 사용한다. 
  * **EX) hotfix-0.1**



## :iphone: Application

 https://github.com/NeighborFree/App


## :computer: Server

 https://github.com/NeighborFree/Server

## :game_die: Blockchain

https://github.com/NeighborFree/BlockChain

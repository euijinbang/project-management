## 1. Gitflow

![git-flow_overall_graph](https://techblog.woowahan.com/wp-content/uploads/img/2017-10-30/git-flow_overall_graph.png)

![image-20220114220039171](Gitflow, Version Control, Commit Messages.assets/image-20220114220039171.png)

- `master` 브랜치는 최종 배포를 위한 용도이다.
- `release` 브랜치로 버젼을 관리한다.
- `develop` 브랜치를 `default` 설정하여 사용한다.
- `feature` 브랜치를 기능마다 생성하여 작업을 진행하고 작업이 완료되면 브랜치를 삭제한다.
  - 각각의 기능은 `conflict` 방지를 위해 백엔드, 프론트엔드를 나눈 상태로 진행해야하며
  - 하나의 브랜치는 한 명이 담당한다.
  - 백엔드 한 명이 기능 하나를 `TEST` 한 후 `develop` 브랜치에 `merge`하면 
  - 프론트엔드가 서버를 내려받아 이어 테스트 후 `develop` 브랜치에 `merge` 한다.

참고 : https://techblog.woowahan.com/2553/



## 2. Version Control

```
v. 1.2.3
```

- `1` : 아주 큰 기능이 바뀔 때이다. 예를 들어 office 2000 이 office 2002로 바뀌는 경우가 있다.
- `2` : 기본적인 기능은 같은데 새 기능이 업데이트 된 경우이다. 예를 들어 커널에 방화벽이 없다가 새롭게 생기는 경우이다.
- `3` : 기능 바뀐것은 없다. 예를 들면 릴리즈 했는데 버그가 생겨 픽스해서 패치한 경우가 있다.



## 3. Commit Messages

- 통일된 commit message 를 작성하자.

![image-20220114213549920](Gitflow, Version Control, Commit Messages.assets/image-20220114213549920-2166079.png)

참고 : https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716



## 4. Code Review

- 코드 리뷰는 주로 시니어에게 `reviewer` 지정을 통해 시행한다.
- `github` 에는 코드 리뷰를 지원하는 다양한 툴이 존재한다.
- (참고) `assignee` 는 `merge` 권한을 가진 사람을 할당한다.


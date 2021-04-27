# Travel-Plan

1. 개발환경
1. 배포전략


## 1. 개발환경
- node.js
- typescript
- react.js


## 2. 배포전략
### 브랜치 설명
<strong>master</strong>
- 실서버에 배포된 가장 최신의 소스를 가지고 있는 브랜치이다.

<strong>develop</strong>
- 개발중인 가장 최신의 소스를 가지고 있는 브랜치이다.

<strong>feature</strong>
- 수정 사항이나 신규 개발건의 경우 develop 으로부터 브랜치하여 개발하는 브랜치다.
- 명명규칙 ex) feature-{JIRA_이슈번호}
- 실서버에 배포가 완료되고 난후 remote의 feature 브랜치는 삭제한다.

### Tagging 방법
```
# 로컬에서 tag 생성전 리모트의 최신 tag 버젼을 조회
$ git ls-remote --tags

# 로컬에서 tag를 생성한다. (여러줄인 경우 -m 옵션을 여러번 작성)
$ git tag -a v1.0.0 -m "* Change number 1" -m "* Change number 2"

# 로컬에서 생성한 tag를 리모트로 전송
$ git push origin v1.0.0
```

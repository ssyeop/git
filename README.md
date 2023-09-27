GIT 배우기
===

Github
---
### github 가입
- [github](http://github.com/)에서 회원가입
- 새로운 Repository(원격저장소) 만들기

    - owner:사용자이름
    - Repository name:중복되지 않는 저장소
    - description: 저장소를 설명하는 요약한줄
    - public/private:공개/비공개 설정
    - add a readme:리드미 파일을 자동으로 추가(체크 비권장)
    - add gitignore:깃저장소에 올리면 안되는 파일의 목록이 담긴 파일
    (해당 파일들은 무시)
    추가하기 (프로그래밍 언어별 기본값)
    - choose s license:오픈 소스에 대한 지적 재산권을 보유하기 위한 파일추가(이후 추가가능)
    - 3가지 파일을 선택하지 않으면 quick setup(CLI명령어)를 볼 수 있다.

git
---
1. 깃 저장소 만들기 명령어: `git init`
2. 깃 추적되지 않은 파일 모두 현재폴더 기준으로 
**스테이징**:
`git commit -m
"커밋 메세지"`



4.  **원격저장 추가하기**
운격저장소 이름, 주소
4. 메인 **브랜치**로 변경하기
  
기본원격 저장소의 이름은 'origin' 기본 브랜치의 이름은 'main'이다.

### 용어 정리
- git: VCS버전 관리 시스템
- github: git으로 관리하는 프로젝트를 원격으로 공유하는 사이트
- GUI:마우스로 화면을 클릭해서
- CLI:명령어를 하나씩 입력해서  사용하는 방식
- commit: 버전관리를 통해 생성된 파일 또는 행위
- log:지금까지 만든 커밋을 모두 확인
- 로컬저장소: 내컴퓨터 안의 git저장소
- 원격저장소: github에 업로드된 git프로젝트
- push: 로컬저장소->원격저장소로 올리는것
- pull: 로컬저장소->로컬저장소로 내려받는것



### 소스트리에 토큰 적용하기

- 최상단 메뉴:도구-옵션-인증
- 계정선택->편집->인증
- p token 선택후 복사한 토큰 붙여넣기

### Git저장방식 알아보기
- git의 저장방식 snapshot
- 차이점만 저장하는 방식 : delta
- 순서
    1. 변경된 파일저장(save)
    2. 스테이지 올림(git add)
    3. 스테이지의 스냅샷을 찍는다. (git commit)

- 깃으로 관리하는 파일의 4가지 상태
   - 추적이 안된상태(untracted)-add가 한번도 없었던 상태
   - 추적된 상태 (track)-add가 한번이라도 된상태
      1. 수정없음:unmodified
      2. 수정함:modified
      3. 스테이지 됨

   - 예시
     - 새로운 파일을 만들었을때
       -untracked(추적안된상태)
    - add를 통해 스테이징
    - commit을 통해 snapshot




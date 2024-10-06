# **오픈소스SW개발론**

### Introduction

-------------
### _Week1-1 강의 개요 (강의계획서)_
3가지 목표를 지향한다.
1. 오픈소스 소프트웽 개발을 위한 기본 개념과 도구, 특히 소스 코드 버전 컨트롤과 패키지 관리, 프로젝트 빌드를 중점으로 배운다.
2. 짝 프로그래밍, 테스트 주도 개발, 행위 주도 개발, 클라우드 기반 **데브옵스**를 공부
3. 새로운 소프트웨어 개발 환경 및 도구를 _스스로 배우는 태도를 배우는 것을 목적_  
[강의 계획서](https://rptbi.jnu.ac.kr/ReportApp/stdhak/reportView.aspx)

-------------
### Week1-2 오픈소스소프트웨어 개요

#### Commercial SW
- 개별 이용허락
- 로열티 지급
- 실행 바이너리만 제공
- 복제, 배포, 수정 불가
- 사용 기간과 목적 제한

#### Open Source SW
- 일괄 사전 이용 허락
- 로열티 없음
- 소스 코드 제공
- 복제, 배포, 수정 허용
- 기간/목적 제한 없음
-------------
### Week2-1 버전 관리 개요
- **Checkin** : 내 작업물 저장소에 올리기
- **checkout, editing** : 저장소에 있는 다른 사람의 작업물 가져오기
- **Diffs** : 다른 사람의 작업물과 나의 작업물 비교
- **Branching** : 기능들이 서로 다른 방향으로 개발되는 경우도 있음 
- **Merging** : 브랜칭된 작업물들을 합치는 기능
- **Conflicts** : 서로 다른 방향으로 개발된 작업물들이 충돌하지 않게 해주는 기능
- **Tagging** : 버전 관리 ex) version1.0 같이
1. #### 중앙 집중형 : 중앙 저장소를 가지고 관리되는 시스템 ex) SVN
2. #### 분산 관리형 : 분산 저장소를 가지고 관리되는 시스템 ex) GIT
-------------
### Week2-2 Git
- Git : 리누스 토르발스가 개발한 분산형 버전 관리 시스템(VCS) 
- **local repository** : 개별 PC에 파일이 저장되는 개인 전용 저장소
- **remote repository** : 파일이 원격 저장소 전용 서버에서 관리되는 저장소
- 작업 공간 : 개인 컴퓨터 환경에서 소스 코드를 편집하는 일반적인 프로젝트 폴
- index : 커밋을 실행하기전, 저장소와 작업공간 사이 존재하는 공간
![오소소1](https://velog.velcdn.com/images/kse3447/post/ada6cffe-2ef7-4e9e-8abf-99c18f608be7/image.png))


-------------
### Week2-3 Github, fork, pull request
fork : 다른 사람의 저장소의 데이터를 내 저장소로 가져오는 기능  
pull request : fork로 가져온 데이터를 수정하고 그것을 원본 저장소로 옮길 때 사용하는 기능

>
즉 Repository에 권한이 없는 사용자가 저장소를 fork하고 fork한 자신의 저장소에 변경 사항을 적용한 후 Push한다.  
이 후 원래 저장소(original repository)에 내 저장소에 있는 브랜치를 Pull Request 한다. 내가 만든 코드가 통과되면 해당 저장소에 Merge 된다.

[My Github Blog](https://github.com/seougmun-01/oss_git_example)

-------------
### Week2-4 Git: Advanced topics

#### git add : 커밋할 목록에 추가  
#### git commit : 커밋 ( 히스토리의 한단위 ) 만들기  
#### git push: 현재까지 역사 (commits) Github 에 밀어넣기  
#### git init : 해당 폴더를 git 초기화  
#### git status : git 상태확인 명령어  
#### git log : 로그를 확인하는 명령어  
#### git diff : commit 이나 branch 사이에 다른점 혹은 파일이나 Repository와 Working space 사이의 다른점을 보여주는 명령어  
#### git remote add origin < 아까복사한 URL> : 새로운 원격 저장소 추가하기  
#### git clone <저장소 url> : 저장소 복제하기  
#### git reset : add한것 취소  
-------------
### Week3     Markdown
**_Italics and Bold_**
- 이탤릭체나 볼드체를 사용하기 위해서는 하고자 하는 말에 ‘_’, ‘**’을 붙이면 된다. Ex) _italics_, **bold**  
- 이탤릭체나 볼드체는 따로따로 쓸 수도 있지만, 같이 사용할 수 있다. Ex) **_italics and bold_**  
 ### Headers
- ‘#’을 사용함에 따라 글자크기를 최대 1단계에서 6단계로 조절할 수 있다.  
- ‘#’을 1개 사용했을 때, 가장 크고, 6개 사용했을 때 가장 작다.  
### Links
- 글자에 링크 삽입을 위해서는 대괄호([])안에 글자를 적고, 소괄호 안에 링크 주소를 적습니다.  
- Ex) [전남대] (https://portal.jnu.ac.kr/Pages/Default.aspx)  
### Images
- 링크 삽입 방법과 비슷하지만 대괄호 앞에 ‘!’가 추가됩니다. 그러나 차이점은 텍스트가 화면에 드러나지 않고 이미지만 드러납니다.
- ![마크다운](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT904XZ8kpOic417aETQDdVWE2u5LpQ6XJhNQ&s)
### Blockquotes
>인용문의 경우 ‘>’을 활용하여 만드는데, 문장의 맨 앞에 추가하여 만들거나, 여러 문단에 나누어져 있는 경우 각 문단의 앞에 ‘>’을 추가하여 만들 수 있습니다.  
### Lists
* 순서가 없는 리스트를 만들기 위해서는 문장 앞에 ‘*’를 붙입니다.(띄어쓰기 필수) 
* 순서가 있는 리스트를 만들기 위해서는 문장 앞에 숫자를 붙입니다.(띄어쓰기 필수)  
### Paragraphs
마크다운에서는 엔터를 한번 눌러서는 줄바꿈이 되지 않고,  
스페이스바를 두번 눌러서 단락을 나눕니다.


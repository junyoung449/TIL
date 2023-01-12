# CLI
|GUI|CLI|
|:---|---:|
|**그래픽**을 통해|**명령어**를 사용하여|
>사용자와 컴퓨터가 상호 작용하는 방식
## GIT BASH 명령어
   * ls *목록 확인*

   * ls -a *숨김파일까지 확인*
   
   * clear *화면 지우기*
   
   * mkdir *make directory, 디렉토리 만들기*
   
      mkdir 폴더명
   
   * cd *change directory, 디렉토리 이동*
   
         cd *위치*
         cd .. *상위폴더로 이동*
   
   * find -name 폴더명 *디렉토리 찾아줌*
   
   *  pwd *print working directory, 절대 경로*
         
          ./ *현재 작업중인 폴더*
          ../ *현재 작업중인 폴더의 부모 폴더*
   
   
* rmdir *remove directory, 디렉토리 삭제*
   
      rmdir 폴더명
   
* rm
      
      -r(recursive) 폴더명 *재귀 명령어, 하위 디렉토리까지 모두 삭제*
      -f(force) 폴더명 *경고문 무시하고 강제삭제*
      -rf 폴더명 *경고문 무시하고 하위 디렉토리 전부 삭제*
* touch 파일 *파일 생성*
* start/open 파일 *폴더,파일을 여는 명령어(windows-start, macOS-open)*
* ctrl + 
  
      ` *terminal on/off*
      b *explorer on/off*
      + number *workspace on*
      / *블럭 주석처리*

# Bash-CLI program

## Markdown
   * 텍스트 기반의 가벼운 마크업 언어
   * 문서의 구조와 내용을 같이 쉽고 빠르게 적고자 탄생

1. ## 헤딩(Heading)
   * #의 개수에 따라 제목의 수준을 구별(h1-h6)

   * 문서 구조의 기본
   * 글자 크기를 키우기 위해서 사용하면 안돼요

2. ## 1.2.3. *-
   * 리스트(List)
   * 순서가 있는 리스트와 순서가 없는 리스트
   * 목록을 표시하기 위해 사용
   * 많이 사용하는 태그 중 하나

3. ## \```code block``` \`inline code block`
   * 코드 블럭(Code Block)
   * 개발자가 마크다운을 이용하는 이유 중 하나
   * 사용하는 프로그램에 따라 특정 언어를 명시하면 구문 강조 지원.

4. ## \[string](url)
      >\[보여지는 부분](url)
   * 링크
   * 다른 페이지로 이동하는 링크를 삽입
   * 필요하다면 파일의 경로를 넣어 다운로드 가능한 링크로 만들 수 있어요.

5. ## \![string](img_url)
   >\[설명](url)
   * 이미지의 너비와 높이는 조절할 수 없음
   * 조절이 필요하다면 HTML 이용해야함

6. ## \*\*Bold** \*italic* \~~strikeout~~
   * 텍스트 강조

7. \---
* 수평선
* 대개 단락을 구분할 때 사용

---
## 참고 자료 https://www.markdownguide.org/cheat-sheet/
---


# Git

## Git 기본기
   * README.md
   * 프로젝트에 대한 설명 문서
   * github 프로젝트에서 가장 먼저 보는 문서

## Repository
   * 특정 디렉토리를 버전 관리하는 저장소
   * git init 명령어로 로컬 저장소 생성
   * .git 디렉토리에 버전 관리에 필요한 모든 것이 들어있음
   * 특정 버전으로 남긴다=commit한다.

|Working Directory||Staging Area||Repository|
|:---|---|---|---|---:|
|작업영역|git add=>|commit으로 남기고 싶은 내용|git commit=>|commit|

   * git status : 현재 상태 확인
   * git commit -m "commit_message" 커밋 메시지는 자세하게!
   * git clone (url) 
      > 다운로드와의 차이점: 다운로드 하면 .git 이 따라오지 않음
   * git restore --staged *file* 
      > Move *Stagged File* to *Working Directory* 
   ---
## *Git Bash로 원격 저장소에 연결하기*
  * mkdir folder
  * git init
  * touch README.md
  * git add README.md
  * git config --global user.email "junyoung449@gmail.com"
  * git config --global user.name "Junyoung"
  * git commit -m "text"
   * git remote add origin *url* 
   * git remote -v 
   * (option)git branch -M main(main으로 이름 변경)
   * git push -u origin main
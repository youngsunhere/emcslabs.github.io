---
layout: post
title: 다섯 줄로 배우는 가장 간단한 Git 사용법
date: 2016-11-30
---

**1) CLONE - 2) cd - 3) ADD - 4) COMMIT - 5) PUSH**

------------------
## 다섯 줄로 배우는 Git 사용법 ##

1. CLONE
	- 서버 상의 저장소(repos) 복제해오기  
	`git clone https://github.com/EMCSlabs/emcslabs.github.io.git`  

	- [참고] 저장소의 주소는 Github repository 오른쪽 상단에서 쉽게 확인 가능!
	![enter image description here](https://lh3.googleusercontent.com/-bd9vv1y2jwA/WD5GVU9BzQI/AAAAAAAAB1E/XTO08-Q77k8CLIwj9CmxUzR6l4xujlBYwCLcB/s0/%25E1%2584%2589%25E1%2585%25B3%25E1%2584%258F%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25B5%25E1%2586%25AB%25E1%2584%2589%25E1%2585%25A3%25E1%2586%25BA+2016-11-30+%25E1%2584%258B%25E1%2585%25A9%25E1%2584%2592%25E1%2585%25AE+12.19.50.png "git_howto_ex.png")

2. 로컬 저장소 속으로!
	- 다운받은 로컬 저장소 안으로 경로 이동하기  
	`cd emcslabs.github.io/`

3. ADD
	- 로컬 저장소의 모든 파일과 폴더를 동기화 대상으로 추가하기 (파일 삭제도 동기화 대상에 포함됨)  
	`git add -A`

4. COMMIT
	- 변경한 내용들을 확정하기 (원격으로 보내기 전에 마지막으로 내용물을 확정하는 단계)  
	`git commit -m "이번 버전에 대한 설명"`

5. PUSH
	- 원격 서버로 버전 발행하기  
	`git push origin master`


----------
### 참조한 사이트 ###
* git을 시작하기 위한 간편안내서 (by. Roger Dudler, 한국어 번역 페이지.):  
<https://rogerdudler.github.io/git-guide/index.ko.html>

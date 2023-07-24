# Git 소개 및 설치

## 01. Git 소개

<img src="./img/git0101.jpg" width="250px">

`Git`은 **Linus Torvalds**가 개발한 버전 관리 시스템(Version Control System)이다.<br>

Git을 통해 소스 코드들을 효과적으로 관리할 수 있다.<br>

1. `버전 관리(Version Control)`: 문서를 수정할 때마다 언제, 무엇을 변경했는지 자세히 기록한다.<br>

2. `백업(Backup)`: 온라인 저장소인 GitHub를 통해, 파일들을 백업할 수 있다.<br>

3. `협업(Collaboration)`: 온라인 저장소인 GitHub를 통해, 편리하게 협업을 할 수 있다.<br>

---

## 02. Git 설치 (Windows)

[https://git-scm.com/](https://git-scm.com/)에 접속해, 운영체제에 맞게 프로그램을 다운로드 한다.<br>

<img src="./img/git0102.png" width="750px">

<br>

라이센스 정보와, 구성요소를 확인한다.<br>

<img src="./img/git0103.png" width="750px">

<br>

기본 편집기로 Vim을 선택하고, 브랜치 이름을 main으로 설정한다.<br>

<img src="./img/git0104.png" width="750px">

<br>

커맨드 라인에서 Git을 사용할 방법과, 보안 서버에 접속하는 방법을 설정한다.<br>

<img src="./img/git0105.png" width="750px">

<br>

보안이 추가된 연결에 연결할 방법과, 텍스트 파일에서 줄 끝부분을 처리하는 방법을 설정한다.<br>

<img src="./img/git0106.png" width="750px">

<br>

터미널 애뮬레이터와 'git pull' 명령을 처리하는 방법을 설정한다.<br>

<img src="./img/git0107.png" width="750px">

<br>

Git 자격 증명 관리자를 선택하고, 파일 시스템을 캐싱하도록 설정한다.<br>

<img src="./img/git0108.png" width="750px">

<br>

제시된 옵션 사용 여부를 선택 후, [Install]을 눌러 설치를 완료한다.<br>

<img src="./img/git0109.png" width="750px">

<br>

설치 후, 윈도우 탐색기에서 [Git Bash]가 정상적으로 실행되면 설치에 성공한 것이다.<br>

<img src="./img/git0110.png" width="750px">

---

## 03. Git 프로그램 종류

사용자가 Git을 쉽게 사용하기 위해, [다양한 종류의 Git 프로그램들](https://git-scm.com/downloads/guis)이 존재한다.<br>

`GUI (Graphic User Interface)` 방식

- **장점**: Git을 쉽게 사용할 수 있다.<br>

- **단점**: 자주 사용하는 기능들만 존재한다.<br>

`CLI (Command Line Interface)` 방식

- **장점**: 익숙해지면 Git을 더 빠르고 다양하게 이용할 수 있다.<br>

- **단점**: 사용법이 어렵다. (Terminal 명령 숙지)<br>

<br>

CLI 방식을 사용하기 위해서는 **Linux**의 기본 명령을 알아야 한다.<br>

---

## 04. Git 환경 설정하기

```bash
git config --global user.name "이름"
git config --global user.email "이메일"
```

Git은 버전을 저장할 때마다, 버전을 만든 사용자 정보를 함께 저장한다.<br>

따라서 Git을 사용하기 전에 사용자 정보(이름, 이메일)를 저장해야 한다.<br>

**[Git Bash]**를 실행하고 위의 명령어를 입력해주면, 사용자 정보 설정이 완료된다.<br>

<br>

`git config`: Git에서 사용자 정보를 설정할 때 사용하는 명령<br>

- `--global`: 현재 컴퓨터에 있는 모든 저장소에서 같은 사용자 정보를 사용하도록 설정하는 옵션<br>

---
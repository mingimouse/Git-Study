# 버전 제외하기 (.gitignore)

## 01. .gitignore

`.gitignore`: 버전을 관리하지 않을 디렉터리나 파일들의 목록을 지정하는 곳<br>

지정된 파일들은 별도의 작업 없이 Git에서 자동으로 버전 관리에서 제외한다.<br>

---

## 02. 사용법

```bash
# .gitignore

# mynote.txt 버전 관리 제외
mynote.txt

# temp 디렉터리 버전 관리 제외
temp/

# .swp 파일들은 버전 관리 제외
.swp
```

.gitignore 파일에 버전 관리를 하지 않을 파일명, 디렉터리명, 확장자를 지정한다.<br>

보통 버전 관리에서 제외하는 파일들은 다음과 같다.<br>

- IDE tool과 관련된 설정 파일<br>

- 언어의 빌드 결과물, 로그, 패키지 관련 파일<br>

- 그 외 프로젝트에서 사용자가 버전 관리에서 제외하고자 하는 파일<br>

---

## 03. gitignore.io

[gitignore.io](https://www.toptal.com/developers/gitignore) 페이지에 접속하면 쉽게 .gitignore 파일을 생성할 수 있다.<br>

검색창에 운영체제, 개발환경(IDE), 프로그래밍 언어를 검색하면 자동으로 .gitignore 파일을 생성해준다.<br>

생성된 파일의 내용을 복사하고 .gitignore 파일에 붙여넣기 하면 된다.<br>

---

## 04. 주의점

### I. .gitignore 작동 조건

.gitignore 파일은 `git add`나 `git commit` 전에 설정되어 있어야 제대로 작동한다.<br>

이미 스테이징이나 커밋이 된 경우, .gitignore가 작동하지 않는다.<br>

```bash
git rm 파일 --cached
```

이미 스테이징을 한 경우, `git rm 파일 --cached` 명령을 사용해 스테이징을 취소한다.<br>

- `git rm 파일 --cached`: 스테이징 취소 & Git에서 변경 사항 추적 X (untracked)<br>

- `git restore --staged 파일`: 스테이징 취소 & Git 변경 사항 추적 O (tracked)<br>

<br>

### II. git add . :vs: git add *

- `git add .`명령 사용 :arrow_right: .gitignore을 **제외**한 모든 파일이 스테이징<br>

- `git add *`명령 사용 :arrow_right: .gitignore을 **포함**한 모든 파일이 스테이징<br>

<br>

### III. ignore된 파일 확인

```bash
git status --ignored
```

`git status --ignored`: ignore 처리된 파일을 확인하는 명령<br>

---
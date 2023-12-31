# Linux 기본 명령1: 디렉터리 관리

## 01. 디렉터리

Windows에서의 `폴더(folder)`를 Linux에서는 `디렉터리(directory)`라고 부른다.<br>

Linux에서 디렉터리를 나타내는 기호는 다음과 같다.<br>

| 디렉터리 관련 기호 | 설명                                  |
| ------------------ | ------------------------------------- |
| **~**              | 홈 디렉터리 (`c/Users/사용자 아이디`) |
| **.**              | 현재 사용자가 작업중인 디렉터리       |
| **..**             | 현재 디렉터리의 상위 디렉터리         |

---

## 02. pwd (print working directory)

```bash
pwd
```

`pwd`: 현재 위치의 경로를 출력하는 명령<br>

---

## 03. ls (list)

```bash
ls
ls -l	# 상세 정보를 함께 표시하는 옵션
ls -al	# 옵션 여러 개를 동시에 사용 가능
```

`ls`: 현재 디렉터리에 어떤 디렉터리나 파일이 있는지 출력하는 명령<br>

이 때, 출력된 이름 뒤에 슬래시(`/`)가 있으면 디렉터리라는 뜻이다.<br>

ls 명령 뒤에 옵션을 추가하면, 파일과 디렉터리를 다양한 형식으로 나타낼 수 있다.<br>

- `-a`: 숨긴 파일이나 디렉터리도 함께 표시하는 옵션<br>

- `-l`: 파일이나 디렉터리의 상세 정보를 함께 표시하는 옵션<br>

- `-r`: 파일의 정렬 순서를 거꾸로 표시<br>

- `-t`: 파일 작성 시간순으로 표시 (내림차순)<br>

---

## 04. cd (change directory)

```bash
cd ~			# 홈 디렉터리로 이동 (c/Users/사용자이이디)
cd ..			# 상위 디렉터리로 이동
cd 디렉터리명	# 해당 하위 디렉터리로 이동
```

`cd`: 디렉터리를 이동할 때 사용하는 명령<br>

---

## 05. mkdir (make directory)

```bash
mkdir 디렉터리명
```

`mkdir`: 현재 디렉터리 안에 새로운 하위 디렉터리를 생성하는 명령br>

---

## 06. rm (remove)

```bash
rm -r 디렉터리명
```

`rm`: 현재 디렉터리 안에 하위 디렉터리를 삭제하는 명령<br>

- `-r`: 삭제하고자 하는 디렉터리 안에 있는 디렉터리와 파일들을 모두 삭제하는 옵션<br>

---

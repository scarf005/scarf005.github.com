---
title: 터미널에서 VS Code 써보기
date: 2022-01-23 21:35:54 +09:00
---

## 사실 vscode는 터미널에서도 쓸 수 있대

어떻게? 터미널에서 `code`를 입력해서!

### 명령어가 없다고 뜨면
```bash
❯ which code
/usr/bin/code
```
가 되는지 확인하고 안 된다면 `PATH`에 vscode 경로 추가해주기

### 실행되자마자 아무 말 없이 꺼진다면
`code --status`로 상황 확인하기, 저장할 디렉토리가 없어서 일어날 수도??

## 어떻게 쓸까

`code [파일 목록]`: 새 vscode 창 열기. 없는 파일이면 새로 만들어 준다


`-s`: 기존 창에서 열기
`-g <파일>:줄 수`: 파일을 열고 그 줄로 이동하기
`-g <파일>:줄 수:열`: 그 다음에 그 열까지 이동하기
`-a, --add <디렉토리>`: 디렉토리 만들기
`-d, --diff <파일> <파일>`: 두 파일 차이 비교하기

`-`: 목록을 표준 입력에서 읽어오기 (예: 'ps aux | grep code | code -')
---
title: 우분투
---

우분투 사용과 관련된 팁!

## 간단 명령어
```bash
# 유저 추가
adduser [user name]

# 그룹에 유저 추가
usermod -a -G [group name] [user name]
    -a : user를 group의 사용자로 추가
    -G : user의 secondary group으로 추가

# 디렉토리 or 파일 권한 변경
chmod -R xxx [directory or file name]
    -R : 하위 폴더, 파일까지 모드 변경
    xxx : 0~7 값으로 모드 변경

# 디렉토리 or 파일 소유자 변경
chown -R [user name] [directory or file name]

# 디렉토리 or 파일 그룹 소유자 변경
chgrp -R [group name] [directory or file name]

# 디렉토리 및 파일의 디스크 사용량을 확인 (Disk Usage)
du -h
    - 사용자 레벨의 프로그램으로 meta data 같은 것들을 반영시키지 못함.
    -h : human readable

# 시스템의 파일 시스템 디스크 공간 사용량을 확인 (Disk Free)
df -h
    - 시스템의 disk allocation map 을 보기 때문에 meta data 를 계산.
    -h : human readable
```



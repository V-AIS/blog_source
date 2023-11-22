---
title: 우분투
---

우분투 사용과 관련된 팁!

## 간단 명령어
```bash
adduser [user name]

usermod -a -G [group name] [user name]
-a : user를 group의 사용자로 추가
-G : user의 secondary group으로 추가

chmod -R xxx [directory or file name]
-R : 하위 폴더, 파일까지 모드 변경
xxx : 0~7 값으로 모드 변경

chown -R [user name] [directory or file name]

chgrp -R [group name] [directory or file name]

du -h
- Disk usage
- 사용자 레벨의 프로그램으로 meta data 같은 것들을 반영시키지 못함.
-h : human readable

df -h
- Disk free
- 시스템의 disk allocation map 을 보기 때문에 meta data 를 계산.
-h : human readable
```



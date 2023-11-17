---
title: 개발 환경 구축
tags: 
  - Setting
---

작성중입니다!

# Python 개발 환경
- Local, virtualenv, Anaconda, Docker


{{< expand "Local">}}
## Local
{{< /expand >}}

{{< expand "virtualenv">}}
{{< /expand >}}

{{< expand "Anaconda">}}

1. 아나콘다 다운로드  

먼저, 아나콘다를 다운로드하기 위해 아나콘다 공식 웹사이트에서 우분투용 설치 파일을 다운로드합니다.

```bash
wget https://repo.anaconda.com/archive/Anaconda3-latest-Linux-x86_64.sh
```
2. 다운로드한 파일 실행 권한 부여  

다운로드한 설치 파일에 실행 권한을 부여합니다.

```bash
chmod +x Anaconda3-latest-Linux-x86_64.sh
```

3. 아나콘다 설치  

이제 아나콘다 설치 파일을 실행하여 아나콘다를 설치합니다.

```bash
./Anaconda3-latest-Linux-x86_64.sh
```
설치 과정 중에는 라이센스 동의, 설치 경로 지정 등의 프롬프트가 표시됩니다. 지시에 따라 설치를 진행합니다.

4. 아나콘다 환경 설정  

설치가 완료되면 아나콘다가 시스템 경로에 추가됩니다. 하지만 새로운 터미널 세션을 열거나 아래 명령어를 입력하여 변경 사항을 적용합니다.

```bash
source ~/.bashrc
```

5. 가상환경 생성 및 관리  

가상환경을 생성하고 관리하기 위해 conda 명령어를 사용합니다.

새로운 가상환경 생성:
```bash
conda create --name myenv
```

여기서 myenv는 새로운 가상환경의 이름입니다. 이 이름을 원하는 대로 변경할 수 있습니다.

가상환경 활성화:
```bash
conda activate myenv
```
필요한 패키지 설치 등의 작업을 위해 가상환경을 활성화한 후, conda install <package_name>과 같은 명령어를 사용합니다.
{{< /expand >}}

{{< expand "Docker">}}
{{< /expand >}}
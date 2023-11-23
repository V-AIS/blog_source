---
title: 개발 환경 구축
tags: 
  - Setting
---

# Python 개발 환경

## Local
{{< details "Detail" >}}
- 사용하는 PC에 Python을 설치하는 가장 기본적인 방법입니다!    

### Ubuntu의 경우
Ubuntu를 사용하실 경우 일반적으로 Python3.X가 설치되어 있습니다!  
터미널에서 `python3`를 입력하여 확인해보세요!

### Window의 경우
[https://www.python.org/](https://www.python.org/) 여기에서 원하시는 버전의 Python을 다운받고 설치합니다!

**사실....Local Python을 쓰는 일은 거의 없을 겁니다...**

{{< /details >}}

여기서부턴 용도에 따라 독립된 가상 환경을 만들 수 있는 방법들입니다!
> Q: 왜....독립된 환경이 필요한가요...?  
> A: 만약 개발 A에선 버전 1의 라이브러리를 필요로 하고, 개발 B에선 버전 2의 라이브러리를 필요로 한다면, 어떻게 이 두 라이브러리를 관리할 수 있을까요? 
> Local Python은 하나인데....어떻게 두개의 버전을 설치할 수 있을까요? 
> 이를 해결하기 위한 것이 **독립된 가상 환경 만들기** 입니다.

## virtualenv
{{< details "Detail">}}
1. Python 설치  
우선 Python을 설치해주세요! (되도록이면 Python 3.X 로....)

2. virtualenv 설치  
```bash
python3 -m pip install --user -U virtualenv
```

3. 가상환경 생성  
``` bash
# 명령어를 실행하면 현재 디렉토리 하위에 `myenv`라는 디렉토리가 생깁니다!
virtualenv myenv
```

4. 가상환경 실행  
``` bash
# 상대 경로를 사용할 수도 있고 절대 경로를 사용할 수도 있습니다!
source myenv/bin/activate
```
가상환경을 활성화한 후, pip install <package_name>과 같은 명령어를 사용하여 패키지를 설치하시면 됩니다.
{{< /details >}}

## Anaconda
{{< details "Detail">}}

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

5. 가상환경 생성
```bash
# myenv 는 마음대로 정하셔도 됩니다.
conda create --name myenv
```

6. 가상환경 실행
```bash
conda activate myenv
```

가상환경을 활성화한 후, conda install <package_name>, pip install <package_name>과 같은 명령어를 사용하여 패키지를 설치하시면 됩니다.
{{< /details >}}

## Docker
{{< details "Detail">}}
여기 적기엔 너무 .... 하드할 것 같습니다. 이건 나중에.... 공부하시는게 좋을 것 같아요...
{{< /details >}}

**추가로 궁금한 사항은 댓글로 남겨주세요!**
---
title: FAQ
weight: 2
---

자주 듣는 질문 모음입니다!

# 환경 설정 관련
{{< details "Windows와 Linux 중 뭘 써야하나요?">}}
```markdown
요즘은 Windows에서도 WSL이 잘 되어있어서 어떤걸 사용하셔도 큰 문제 없습니다.  
그래도 전 Linux 사용하겠습니다...
```
{{< /details >}}

{{< details "nvidia-smi에 CUDA 버전이 나와요! CUDA 설치한거 맞나요??">}}
```markdown
아닙니다.  
`nvidia-smi`에 나오는 `CUDA Version`은 현재 드라이버와 호환되는 최신 버전의 CUDA 정보입니다.  
CUDA는 `nvcc --version`으로 확인하셔야합니다.  
```
{{< /details >}}

{{< details "CUDA를 설치했는데 `nvcc --version`을 해도 명령어가 동작을 안해요!">}}
```markdown
설치를 잘못하셨다는 의미입니다.  
혹시나 다음과 같은 작업을 잊으신건 아닐까요? 
`export PATH={cuda bin 경로}:$PATH`  
`export LD_LIBRARY_PATH={cuda lib64 경로}:$LD_LIBRARY_PATH`  
~/.bashrc 에 위 내용이 적혀있는지 확인해보세요!
```
{{< /details >}}

# 이론 & 실전 관련

{{< details "Computer Vision 공부를 하려고 하는데요! 어떤 책을 보면 좋을까요?">}}
[서적 모음](../../2.Study/legacy/book_recommend/)
```markdown
`2.공부자료/N.Legacy/서적 모음`게시글에서 디지털 영상처리, 컴퓨터 비전 추천드립니다.!
```
{{< /details >}}

{{< details "OOM(Out Of Memory)를 해결하는 방법에는 어떤게 있을까요?">}}
```markdown
1. 상위 GPU로 변경
2. 배치 사이즈 줄이기
3. 모델 사이즈 줄이기
4. 입력 사이즈 줄이기
5. Gradient Accumulation 사용하기 (추후 포스팅 예정)
6. Mixed Precision 사용하기 (추후 포스팅 예정)
...

물론 더 있겠지만.... 여기 까지만 적겠습니다.  
추가하고 싶으신 내용이 있다면 댓글로!

```
{{< /details >}}


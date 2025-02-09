# 어디서나 Ubuntu VM을 사용하는 방법 Multipass

macOS나 Windows에서 Ubuntu VM 사용하고 싶으신 적이 있나요?
Multipass를 사용하면 빠르고 간단하게 Ubuntu VM을 생성할 수 있습니다.

## Multipass 설치

Multipass는 macOS, Windows, Linux에서 사용할 수 있습니다.
[공식 홈페이지](https://canonical.com/multipass/install)에서 다운로드 받아 설치할 수 있습니다.

설치가 완료되면 Multipass 어플리케이션을 실행합니다.



## 어플리케이션을 활용한 Multipass로 Ubuntu VM 생성



위와 같은 방법으로 Ubuntu VM을 생성할 수 있습니다.


## 명렬중을 통한 Multipass로 Ubuntu VM 생성

먼저, Multipass를 통해 현재 사용 가능한 이미지를 확인합니다.

```bash
multipass find
```

사용 가능한 이미지를 확인한 후, 아래와 같은 명령어를 통해 VM을 생성할 수 있습니다.

```bash
multipass launch <image> --name <vm-name> --memory <memory-size> --disk <disk-size> --cpus <cpus>
```

그럼 현재 가장 최신 버전의 Ubuntu LTS를 사용하고 memory 2G, disk 10G, cpu 2 를 가지는 `lts-vm`이라는 이름의 VM을 만들어 봅시다.

```bash
multipass launch lts --name lts-vm --memory 2G --disk 10G --cpus 2
```


# Linux Core Concepts
## Linux Kernel
Linux Kernel은 OS의 핵심요소 중 하나.</br>
Linux Kernel은 크게 4가지 핵심적인 일을 수행한다.
1. Memory Management
2. Process Management
3. Device Drivers
4. System Calls and Security

또한 Linux Kernel은 Monolithic하고 Modular한 특징을 가지고 있다.
## Linux Kernel 정보 얻기
```bash
~/D/P/Linux ❯❯❯ uname
Darwin
```
`uname`을 치면 어떤 Kernel을 사용하는지 알 수 있다.
```bash
~/D/P/Linux ❯❯❯ uname -r
19.6.0
```
`uname -r`은 Kernel의 정보까지 알려준다.
## Memomry Management

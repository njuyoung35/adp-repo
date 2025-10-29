## 프로젝트 구조 알아가기

### misys:forza 도커 이미지로 빌드되는 / 경로 구성 알아가기

```
19G     .
12G     ./usr
  ㄴ 기본 시스템 패키지, 개발 도구, 컴파일러 등이 설치됨
5.4G    ./home
1.7G    ./opt
  ㄴ 1.4GB짜리 nvidia 포함
  ㄴ 343MB짜리 ros 포함
604M    ./root
  ㄴ 그냥 캐시 정도밖에 없음..
129M    ./var
  ㄴ 가변 데이터 저장 (로그, 캐시, 스풀 등)
3.4M    ./etc
1.5M    ./run
740K    ./tmp
12K     ./media
4.0K    ./srv
4.0K    ./mnt
4.0K    ./boot
0       ./sys
0       ./proc
0       ./dev
```

#### /usr에 대하여

```
12G     .
6.5G    ./local
  ㄴ 4.7GB짜리 cude-12.4 포함
3.7G    ./lib
  ㄴ 2.3GB짜리 x86_64-linux-gnu 포함 (라이브러리, 동적로딩 .so 파일들)
495M    ./share
395M    ./include
129M    ./bin
6.4M    ./sbin
4.0M    ./src
1.6M    ./libexec
4.0K    ./libx32
4.0K    ./lib64
4.0K    ./lib32
4.0K    ./games
```

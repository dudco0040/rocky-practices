## git 2.45.0 설치

1. 의존성 라이브러리
```sh
# yum -y install curl-devel
# yum -y install expat-devel
# yum -y install gettext-devel
# yum -y install openssl-devel
# yum -y install zlib-devel
# yum -y install perl-devel
```

2. 다운로드
```sh
# wget https://mirrors.edge.kernel.org/pub/software/scm/git/git-2.45.0.tar.gz
```

3. 압축 풀기
```sh
# tar xvfz git-2.45.0.tar.gz
```

4.소스 디렉토리 이동 - 작업할 디렉터리
```sh
  # cd git-2.45.0
```

5. configure build Environment    // configure: 컴파일러가 빌드할 수 있는지 확인, 
```sh   
# ./configure --prefix=/usr/local/poscodx/git-2.45.0
```

6. 빌드
```sh
# make all
```
   
7. 설치 - 실행 후 나오기
```sh   
# make install
```

8. 링크
```sh   
# cd /usr/local/poscodx/
# In -s git-2.45.0/ git
```

09. 설정(/etc/profile)
```sh
export PATH=$PATH:
```

10. 확인
```sh
# source /etc/profile   
# git --version
```

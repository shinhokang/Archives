# LG G2 안드로이드폰 리눅스 서버로 만들기

## 사용기기

* Model: LG G2, F320S(SKT)
* OS Version: 4.4.2

### 순서

1. 루팅 - Root 권한 얻기
2. 필요없는 앱 삭제 (optional)
3. 리눅스 - Ubuntu 설치



## 1. 루팅 - Root 권한 얻기

### IO root 이용
> [http://forum.xda-developers.com/showpost.php?p=48709232](http://forum.xda-developers.com/showpost.php?p=48709232)

* Download: `http://downloads.codefi.re/autoprime/LG/ioroot/ioroot.zip`
* Mac에서도 실행 가능

1. `chmod +x ioroot.sh`
2. `chmod +x ioroot.tool`
3. `ioroot.tool` 실행

루팅까지 완료됨


## 필요없는 앱 삭제 (Optional)

Install [System app remover (ROOT)](https://play.google.com/store/apps/details?id=com.jumobile.manager.systemapp).


## 리눅스 - Ubuntu 설치

### Linux deploy 앱을 이용한 설정 및 설치
> [https://opentutorials.org/module/2113](https://opentutorials.org/module/2113)  
BusyBox 설치 후 linux 설치. SSH 설정 및 연결까지.


#### ssh 연결 후 Locale setting warning 발생 시 

```
$ sudo locale-gen en_US.UTF-8
Generating locales...
  en_US.UTF-8... done
Generation complete.

$ sudo dpkg-reconfigure locales
Generating locales...
  en_US.UTF-8... done
Generation complete.
```

`/etc/default/locale` `/etc/environment` 파일 변경. 아래 줄 추가

```
LANG=en_US.UTF-8
```


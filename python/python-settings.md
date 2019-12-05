
#우분투 리눅스에서 파이썬 설치

우분투(LINUX) 설치환경 : Ubuntu 리눅스 16.04.3 LTS버전에서 설치가능

'''bash
$ sudo apt-get install python3' 
$ sudo apt-get update'
$ sudo apt-get upgrade python3'
'''

현재 설치되어 있는 파이썬 버전을 확인해보기
'''bash
$ python3 --version 
'''

최신버전으로 업그레이드 했는데 이전 버전을 계속 가리키고 있다면.. 
아래의 도큐멘트를 확인해보자

# 우분투 16.04에서 Python3.6사용하기 
- 참고 : 개똥이야기 블로그 [Ubuntu 16.04에서 Python3.6 사용하기](https://unipro.tistory.com/237)

Ubuntu 16.04에는 써드파티 PPA를 추가해야 python3.6을 설치할 수 있다. 
'''bash
'sudo add-apt-repository ppa:jonathonf/python-3.6'
'''

**Python3.6을 설치한다**

'''bash
$ sudo apt-get update
$ sudo apt-get install python3.6
'''

**현재 지금 계속해서 3.6이 설치가 안되고 있는 상항 **
The repository 'http://ppa.launchpad.net/nvbn-rm/ppa/ubuntu xenial Release' 이 에러를 계속해서 못 잡고 있는 상황 
- 써드파티를 추가하고 sudo apt-get update로 진행하면 문제가 난다. 
- 아래의 방법으로 파이썬 버전 설정모드를 통해 할 수 있었음


### After installing Python3.6

'''bash
$ sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.5 1
$ sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.6 2
'''

현재 설치된 파이썬 버전에서 선정할 수 있게 세팅하기 
'''bash
$ sudo update-alternatives --config python3 
'''

Then select the /usr/bin/python3.6 -- automode in choices menu

Now you can switch between Python2.7.12 and Python 3.6.8


<!-- Markdown syntax for image -->
<!-- ![사진이름](사진경로) -->


# MacOS X에서 개발환경 세팅하기 

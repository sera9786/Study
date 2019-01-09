Study 

IT에관한 여러분야 에대해 기록해두고 복습을 위한 레퍼지스토리입니다 



## 배경지식

### 백엔드와 프론트의 차이

음악에서 비유하자면 백엔드는 비트나 드럼이고 프론트는 가수 또는 댄서이다 

사람들이 보는것은 댄서나 가수를보고 환호를하겠지만 비트나 악기들이 뒷받침하지않으면 좋은 공연이 될수없다 

백엔드는 겉으로 잘들어나지않아 사람들이 알수없다 하지만 몇만명이 서버에 접속해도 멈추지않게 내면적인 부분까지 자세히 봐야한다

프론트는 우리가 웹페이지를 들어갔을때 보이는 것들을 만드는 사람이다 백엔드에 비해 쉬워 보일수있지만 둘다 조금씩해봤을때 나는 개인적으로 프론트가 더어려웠다 프론트는 사용자가 편하게 사용할수있도록 배치를 잘해야하고 크기나 색등 많은것들을 신경써야한다.



## 프레임워크(Framework)

간단하게 말하면 프로그램의 기본구조 라고할수있다 건축에 비유하자면 건축물을 지을때 땅이 평평해야하고 기본적인 뼈대가 있어야한다 이런것들을 프레임워크라 생각한다 

#### 프레임워크 예시

* [Spring](https://spring.io/) - Java
* [Django](https://www.djangoproject.com/) - python
* [Angularjs](https://angularjs.org/) - Javascript
* [Larave](https://laravel.com/) - PHP

한언어에는 여러 프레임워크가있다 먼저생각 나는것을 먼저적은것이므로 굳이 꼭 작성해둔것을 쓸필요가없다 여러프레임워크를 써보고 여러언어들을 사용해 개발을 해보는것이 중요하다 언어는 도구일뿐이다.



## 아키텍처(Architecture)

프레임워크와 비슷하게 아키텍처도 뼈대라 말할수있다 하지만 프레임워크와 분명히다르다

아키텍처는 어떤 프로그램을 만들때 그에관한 설계도라 말할수있다 프레임워크에선 건물을 지을때 화장실을 기본적으로 만들어놓을순있지만 아키텍처에선 화장실이있다고 명시 되지않을수도있다 



## 플랫폼 (Platform)

쉽게 프로그램 실행 환경이다 자동차를 만들고 실험주행해볼땐 도로나 사막등등 여러곳에서 쓰임에따라 환경이 달라지듯 프로그램도 환경이 필요하다 

플랫폼은 같은 영역에도 다양한 목적과 가치로 많이 만들어지고 있으며 모든 플랫폼에서 실행되도록 개발하기는 어렵다. 프로그램의 목적에 맞도록 플랫폼을 선택하는 것이 중요합니다.

#### 플랫폼 예시

* window,Linux,macOS등 OS는 모두 플랫폼이다.
* 어플을 다운받는 구글플레이,앱스토어등 모두 플랫폼
* Java같은경우 OS의 제약이없지만 실행을위해선 JVM(Java Virtual Machine, 자바가상머신) 위에서 실행해야하기때문에  java플랫폼이필요함.

## 라이브러리(Library)

프로그램을 개발할때 필요한 기능들이다. 자동차에선 바퀴나 핸들을 예시로들수있다

한프로그램에서 로그인하는 기능이나 위치를 찾는 기능들을 반복으로 코드작성하는것을 없애기위해 호출하여 사용할수있도록 Class나 Funtion 으로 만들어진것이다


## IDE(Integrated Development Environment,통합개발환경)

코딩,컴파일등등 프로그램을만들때 거의모든 개발환경을 관리해준다.

java - [이클립스](https://www.eclipse.org), [intellij IDEA](https://www.jetbrains.com/idea/)

python - [pycharm](https://www.jetbrains.com/pycharm/)

js(javascript) - [Webstorm](https://www.jetbrains.com/webstorm/), [Visual Stdio Code](https://code.visualstudio.com/)

C, C++ - [dev c++](https://sourceforge.net/projects/orwelldevcpp/), [Visual Stdio](https://visualstudio.microsoft.com/ko/vs/)

다른언어들도 여러 IDE를 갖고있다 자바같은 경우는 이클립스를 조금써보고 intellij로 넘어가는것을추천한다 

intellij가 좋긴하지만 문법이 자동완성되기 때문에 편하지만 문법의 형태를 잘익히기어렵다. 

  ## HTTP(Hyper Text Transfer Protocol)

데이터를 주고받는 프로토콜.

프로토콜이란 어떻게 통신을할것인가에대한 규약이다

HTTP는 웹개발자라면 꼭알고있어야한다고 한다 서버를 관리하면서 통신을 어떻게하는지알고 혹시라도 그과정에서 오류가있을수도있기때문에 특히나 백엔드 개발자들에겐 중요하다

#### HTTP의 특징

* HTTP 메시지는 HTTP 서버와 HTTP 클라이언트에 의해서 해석이 됩니다.
* TCP/IP를 이용하는 응용 프로토콜(application protocol)입니다.

* HTTP는 연결 상태를 유지하지 않는 비연결성 프로토콜입니다. (이러한 단점을 해결하기 위해 Cookie와 Seesion 등장)

* HTTP는 연결을 유지하지 않는 프로토콜이기 떄문에 요청/응답(request/response) 방식으로 동작합니다.

![](C:\Users\DSM2018\AppData\Roaming\Typora\typora-user-images\1546572368478.png)

HTTP는 이런식으로 동작하는데 프로토콜에는 많은 형식이있다 



## 웹 서버

* 하드웨어 측면에서 web server는 website의 컴포넌트 파일들을 저장하는 컴퓨터이다. ( 컴포넌트 파일에는 HTML 문서, images, CSS stylesheets,, 그리고 JavaScript files가 있습니다.) 그리고 이 파일들을 최종 소비자의 디바이스에 전달합니다. web server는 인터넷에 연결되어 있고, mozilla.org와 같은 domain name을 통해 접속될 수 있습니다.

* 소프트웨어 측면에서, web server는 기본적으로 웹 사용자가 어떻게 호스트 파일들에 접근하는지를 관리합니다. 이 문서에서 web server는 HTTP서버로 국한합니다. HTTP 서버는 URL(Web addresses)과 HTTP(당신의 브라우자거 웹 페이지를 보여주기 위해 사용하는 프로토콜)의 소프트웨어 일부입니다

* 기본원리

가장 기본적인 단계에서, 브라우저가 웹 서버에서 불려진 파일을 필요로 할때, 브라우저는 HTTP를 통해 파일을 요청합니다. 요청이 올바른 웹 서버(하드웨어)에 도달하였을 때, HTTP 서버(software)는 요청된 문서를 HTTP를 이용해 보내줍니다. 

![](C:\Users\DSM2018\AppData\Roaming\Typora\typora-user-images\1546999710222.png)

## 동적인 웹페이지


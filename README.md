# my-projects
지금까지 진행했던 프로젝트들을 정리합니다

<div id="done-projects">

## Done

### [pr-archiving, Github PR을 모두 저장할 수 있어요](https://github.com/shinkeonkim/pr-archiving)

- 특정 유저가 작성한 Repository의 Github PR 목록을 가져옵니다. 각 PR 상세 페이지 및 files 페이지의 스크린샷을 저장합니다.

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 특정 Repository에서 기여한 내용들을 한번에 모아두고 싶다는 지인들의 니즈

#### 🍿 What & How
- Github PR의 경우, 계정 로그인 및 2FA 인증도 된 이후에 확인할 수 있음을 고려해야 했다.
  - -> 크롬 원격 디버거 모드로 실행 후에 해당 브라우저를 사용하자
- Load more… 및 Show Resolved 등으로 가려져 있는 부분도 처리한 후 정보를 모으고 싶다.,
  - 해당 버튼들을 처리하고 스크린샷을 찍도록 로직을 추가하자

</details>

### [build-testing, Docker 이미지 빌드 후 dockerhub에 올리기](https://github.com/shinkeonkim/build-testing)
- dionysus 프로젝트를 진행하면서 필요한 과정이었는데, 프로젝트에 도입하기 전에 한번 실험해보고 싶었다.  

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- dionysus 프로젝트를 진행하면서 필요한 과정이었는데, 프로젝트에 도입하기 전에 한번 실험해보고 싶었다. 

#### 🍿 What & How
- 간단한 Python Docker container를 dockerhub에 올렸다.

</details>

### [fxck-pdf, PDF 파일에 대한 다양한 기능을 제공하는 GUI 프로그램](https://github.com/shinkeonkim/fuck-pdf)

- PDF 병합 기능, PDF 페이지 삭제 기능, 홀수 페이지 / 짝수 페이지 PDF 파일 병합 기능, PDF 페이지 회전 기능을 제공한다.

<details>
  
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 단순한 PDF 병합, 페이지 삭제를 많이 할 일이 있었지만, 유료 툴을 쓰고 싶지는 않았다.

#### 🍿 What & How
- PDF 문서에 대한 처리가 필요했다.
  - 직접 구현하는 것도 좋지만 라이브러리를 이용해서 빠르게 구현하고 싶었다.
  - -> pypdf2를 활용하자.

</details>

### [amry-tiger, 당신의 군대 일정 Github에도 공유해요](https://github.com/shinkeonkim/army-tiger)

- 🪖 군대 일정을 Github 프로필에 남겨둘 수 있어요

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 갑작스럽게 군대를 가면서, 지인들이 입대, 전역 일정을 계속 물어봤다.
- Github 페이지를 통해 관련 일정을 바로 확인할 수 있게 해주고 싶었다.

#### 🍿 What & How
- ![image](https://github.com/user-attachments/assets/2f894503-0d5f-4182-bca9-f8ddef865ff1)
- Gist에 관련 글을 매일 갱신하게 해야 했다.
  - -> Github Actions를 활용하자.
</details>

### [Algo Sports Front](https://github.com/Algo-Sports/algo-sports-front)

### [khonshu - 오늘의 달 모양은?](https://github.com/shinkeonkim/khonshu)
- 오늘의 달 모양을 보여주는 웹 페이지

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- [문나이트 드라마](https://www.disneyplus.com/ko-kr/series/moon-knight/4S3oOF1knocS)를 보다가, 대뜸 달 모양에 집중하게 되었다.
- 하늘을 보러 나가지 않으니, 안에서라도 달 모양을 보자고 생각해서 만들게 되었다.

#### 🍿 What & How
- 달 모양을 만들어야 했다. 관련 글을 찾아보았고 거의 그대로 구현했다.
- 날짜를 임의로 조절하여 보는 기능도 추가하면 좋을 것 같긴 하다.

</details>

### [mooyaho - 무야호 짤 생성기](https://github.com/shinkeonkim/mooyaho)
- 무야호 대사 대신에 다른 글자를 넣어 이미지를 만들 수 있는 웹 페이지이다.

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 무야호 밈이 너무 유행하여, 한번 짤 생성기를 만들어볼까? 라는 단순한 생각에서 시작했었다.

#### 🍿 What & How
- Vue.js를 한창 쓰고 있었기 때문에 바로 도입해서 사용해보았다.
- 현재는 Vue.js 관련 내용을 CDN으로 불러오지 못해서 오류가 나 사용이 안된다.

</details>

### [Xaskify, 페이지 내의 글자를 모두 마스킹하자](https://github.com/shinkeonkim/xaskify.git)

- 아래와 같이 특정 dom 객체의 하위 요소의 텍스트를 모두 원하는 글자로 마스킹할 수 있게 하는 npm 패키지다.
```js
import xaskify from "xaskify";
xaskify(document.getElementsByTagName("body")[0], "X");
```

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 웹 페이지 스크린샷을 찍는 중에도, 일부 개인정보나 민감한 정보가 나오는 상황이 애매했다.
- 그렇다고 그때그때 일일이 가리는 작업을 하기에도 애매해서 해당 패키지를 사용했다.

#### 🍿 What & How
- 모든 요소가 다 마스킹되어야 한다.
  - -> 재귀적으로 자식 객체를 탐색하며 모두 마스킹시키자.
- 크롬 익스텐션으로 만들어보면 좋을 것 같다.
  - 중단됨
</details>

### [paeon, 사업자등록번호와 상호명으로 검색하는 서비스](https://github.com/shinkeonkim/paeon)

- 공공데이터를 이용해 사업자등록번호 또는 상호명을 통해 기업 정보를 확인하는 서비스

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 그랩 채용서비스 내의 구조 상 해당 정보들을 검증하고 다시 입력하는 과정을 내부 운영자가 하고 있었다. 근데 정확한 문자를 입력해야 하는 상황인데 계속 실수가 발생할 여지가 많았던 굉장히 불편한 과정이었다.


#### 🍿 What & How
- 모든 회사의 데이터를 가져와야 한다.
  - 꼭 주기적으로 돌 필요까지는 없다고 생각했다.
  - 이에, 모든 회사 정보를 reload하는 별도 util과 이를 이용하는 어드민 액션을 추가했다.

</details>

### [is_likelion, 이 문자열은 멋쟁이사자처럼인가?](https://github.com/shinkeonkim/is_likelion)

```py
from is_likelion import is_likelion

is_likelion("likelion") # True
is_likelion("LikeLiOn") # True
is_likelion("멋쟁이사자처럼") # True
is_likelion("lion") # False
```

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 멋쟁이사자처럼 활동중 python 패키지를 만들어보는 예제를 만들어 보려 했다.

#### 🍿 What & How
- pypi에 패키지를 배포했다.
- 간단한 CI 환경으로 구성해서 사용하고 싶었다.
  - -> travis를 사용했다.
  - github action으로 바꾸어 사용해도 될 것 같다.

</details>

### [move it!, 빨간 점을 피해 계속해서 상자를 움직여라](https://github.com/shinkeonkim/move-it)

- 간단한 게임 요소를 웹 페이지에서 구현해본 토이 프로젝트

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 드래그 앱 드랍으로 만들만한 게임적 요소를 생각해봤다.

#### 🍿 What & How
- 사용자가 계속 이걸 하게 될만한 요소는 없을까?
  - -> 위에 계속해서 시간을 보여주면서 더 오래 버티려고 노력하게 만들었다. 

</details>

### [github-repository-start-date-checker, 특정 일자를 기준으로 Repository가 생겼는가 검증](https://github.com/shinkeonkim/github-repository-start-date-checker)

- Github Repository의 목록이 주어졌을 때 특정 일자 이후로 만들어졌는지 검증하는 프로젝트

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 해커톤 진행 중에 이전부터 개발이 진행되었지 않다는 최소한의 제약으로 Github Repository의 생성일자를 검증하기로 했다.

#### 🍿 What & How
- 각 레포지터리의 정보는 어떻게 가져오지?
  - -> github에서 제공하는 API를 이용해서 처리하자.

</details>

### [simulate doves hawks](https://github.com/shinkeonkim/simulate-doves-hawks)

- [이 영상](https://www.youtube.com/watch?v=YNMkADpvO4w)의 내용을 직접 시뮬레이션 해보자

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- [이 영상](https://www.youtube.com/watch?v=YNMkADpvO4w)의 내용을 보다가 직접 시뮬레이션 해보고 싶다고 생각했다.

#### 🍿 What & How
- 간단하게 변인들을 수정하고 싶었다.
  - PyQT GUI를 통해 쉽게 바꿔가며 사용할 수 있도록 했다.

</details>

### [Lotteng](https://github.com/hyeoneedyou/lotteng)

- 2020 멋쟁이 사자처럼 X Lotte 8기 해커톤 프로젝트
- 동상 수상

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 2020 멋쟁이 사자처럼 X Lotte 8기 해커톤에 참가해 진행하게 된 프로젝트

#### 🍿 What & How
- 간단하면서도 빠르게 웹 개발을 진행해야 했다.
  - AWS EC2, nginx, gunicorn에 배포하는 과정으로 처리했다.
  - 추가적인 배포가 반복되거나 유지보수하는 경우가 적기에 인프라는 간소화시켰다.

</details>

### [alcolpedia](https://github.com/kkIIun/alcolpedia)

- 술자리 문화, 술게임 등을 소개하는 웹 서비스

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 멋쟁이사자처럼 내에서 프로젝트 진행 주제가 필요했음. 마침 술을 마시던 중에 팀원이 프로젝트 주제를 떠올렸고, 같이 참여해서 진행했다.

#### 🍿 What & How
- 내부 컨텐츠
  - 직접 사진을 제작하거나 녹음해서 제공을 했다.

</details>

### [tabular method cli](https://github.com/shinkeonkim/tabular-method-cli)

- 국민대학교 논리회로설계 강의 시간 중, 배운 tabular method를 구현한 CLI 프로그램

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 국민대학교 논리회로설계 강의 시간 중, 배운 tabular method를 과제로 구현하게 되었다.

</details>


### [3d-printer-calibration-program, daVinci 1.1 plus 3D priter calibration을 위한 CLI 프로그램](https://github.com/shinkeonkim/3d-printer-calibration-program)

- daVinci 1.1 plus 3D priter calibration을 도와주는 CLI 프로그램

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 고등학교 3D Printer 방과후 수업 중 느낀 daVinci 1.1 plus calibration 과정의 불편함을 해결하기 위해서 만들었다.

#### 🍿 What & How
- 조정 나사의 위치와 위치 측정 센서의 위치가 서로 상이한 위치에 있고, 평평함을 조정하기에 불편한 방식이었다.
  - 간단한 수식을 정리하고 프로그램에 반영
- 어떤 식으로 돌리는게 최적일지 고민
  - 간단한 BFS 알고리즘과 백트래킹을 활용해 처리
  - 지금보면 코드가 굉장히 안좋게 설계된 것으로 보이지만,, 그 당시의 코드를 보관하는 중

</details>

### [Sellon](https://github.com/bunderLikeLion/sellon_frontend)

- 멋쟁이 사자처럼 10기 전체 해커톤
- 약 900 명 참여, 150팀 중 동상 수상
- 현대 사회에서 지속적으로 쌓여가는 잡동사니에 대한 공간적 문제를 해결 하고자 하는, 기존 물품과 돈이 거래되는 시장에서 탈피하여 본인에게 현재 필요없는 잡동사니와 잡동사니를 경매식으로 교환하는 플랫폼

<details>
<summary>
  자세한 내용 보기
</summary>

#### 🍿 What & How
- 간단하게 개발을 빠르게 해야 하는 상황이었음
  - 기존에 만들어둔 dpd template을 참고하여 프로젝트 구성
- 해커톤 발표시 부하가 있을 수 있다.
  - 부하를 줄이기 위해 webapp container 추가 고려했지만 큰 부하없는 것으로 확인하여 진행하지 않음.

</details>

### [TTL, Today They Learned](https://github.com/today-they-learned/ttl_api)

- 모든 TIL을 한 곳에서 모아보세요. 📚

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- TIL 글들을 한 곳에서 모아서 볼 수 있는 서비스를 만들어 보자.

#### 🍿 What & How
- 백엔드와 프론트엔드 별도 개발
  - -> DRF 를 활용한 API 개발
- 디자이너/기획자가 별도로 없었음.
  - 디자이너/기획자의 role을 수행하면서 백엔드 개발 병행

</details>

### [PeacePiece](https://github.com/today-they-learned/peacepiece_api)

- 일상생활 속 환경을 위한 활동을 기반으로 가상공간을 꾸밀 수 있는 웹플랫폼

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- TTL 프로젝트를 같이 진행한 팀원들과 추가적으로 프로젝트를 진행하고자 함.

#### 🍿 What & How
- 백엔드와 프론트엔드 별도 개발
  - -> DRF 를 활용한 API 개발
- 디자이너/기획자가 별도로 없었음.
  - 디자이너/기획자의 role을 수행하면서 백엔드 개발 병행

</details>

### [peachpitch](https://github.com/shinkeonkim/peachpitch)

- pyqt를 이용한 뮤직 플레이어

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- PyQT를 활용하는 강의 이후 관련 프로젝트 진행을 하게 되었다.

#### 🍿 What & How
- 음악을 가져올 소스가 필요했다.
  - 해당 프로젝트가 금전적인 목적이 아니었기에 youtube API를 활용하는 파이썬 패키지를 가져와서 음원을 받아왔고 이를 재생하게 했다.
- 음원 재생 및 별도 조작 필요
  - QtPlayer의 API를 적극 채용해서 사용했다.

</details>


</div>

<div id="in_progress-projects">

## In Progress

### [Memez 백엔드 프로젝트 - Dionysus](https://github.com/meme-party/dionysus)

- 

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 

#### 🍿 What & How
- 

</details>

</div>

<div id="what_if-projects">

## What If? (더 개선할 수 있지 않을까 싶지만, 핵심 기능은 완성했다.)

### [BOJ to PDF, 백준을 PDF 파일로 변환](https://github.com/shinkeonkim/boj-to-pdf)
- 백준 문제 목록을 받아서, 하나의 PDF 파일로 변환해주는 python 스크립트

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 백준 문제를 버스/지하철에서 주로 푸는데, 메모와 웹 브라우저를 번갈아가며 보는게 불편했다.
- PDF 파일로 저장하여 보면 참 편할 것 같았다.

#### 🍿 What & How
- 백준 페이지들을 PDF로 변환해야 한다.
  - -> BeautifulSoup4를 활용하여 웹 페이지 접근 후 PDF로 추출하자.
- 동시에 여러 페이지를 처리하고 싶다.
  - -> asyncio 도입

</details>

### [가위바위보 시뮬레이터, 가위바위보가 움직이면서 싸우면 누가 이길지 예측해보자](https://github.com/shinkeonkim/rsp-simulator)

- 단순한 시뮬레이션 웹 페이지

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- [마플 - 가위바위보!!!!](https://www.youtube.com/watch?si=bn4ldlUjgo6E0Bef&v=E1EgJYfBv-Y&feature=youtu.be) 을 보고, 웹 페이지에서도 구현할 수 있지 않을까? 싶었다.
- 그리고 좀 더 다양한 변수를 도입해볼 수 있지 않을까 궁금했다.

#### 🍿 What & How
- 각 객체들이 부딪쳤을 때의 연산이 필요하다.
  - -> tick마다 계속 연산을 하는 방식으로 일단 구현하자.
  - -> 이후 최적화를 할 방안이 있는지 고민하자
- 더 많은 변수
  - 속도, 시뮬레이션 속도 등을 추가했다.
  - 이후 추가하고 싶었지만 시간을 더이상 투자하지 않았다..

</details>

### [what-did-you-do-today, 당신은 오늘 백준을 풀었는가? (알고리즘스터디 내 활용)](https://github.com/shinkeonkim/what-did-you-do-today)

- 알고리즘 스터디 내에서 매일 1일 1문제를 풀기 위해서 자동으로 체크해주는 웹 서비스를 만듬
- 그리고 벌금을 자동으로 책정하여 대시보드로 보여줌

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 알고리즘 스터디 내에서 매일 개인의 기록을 확인하는게 힘들었기 때문에

#### 🍿 What & How
- 매일 정각마다 기록을 확인하는 과정이 필요했음.
  - cron이나 별도 job을 통해 돌릴 수 있었지만 더 간단하게 인프라 없이 해결할 방법을 고민했음.
    - -> github actions에서 trigger로 schedule을 추가해두고 특정 키와 함께 요청을 보내면 정보 갱신을 하도록 했음

</details>

### [basic_django_template, 같은 이름으로 생기는 django-admin startproject가 싫다](https://github.com/shinkeonkim/basic_django_template)

- 프로젝트명과 앱명이 같은 이름으로 생기는 django-admin startproject가 싫었기에 만든 템플릿 프로젝트

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 프로젝트명과 앱명이 같은 이름으로 생기는 django-admin startproject가 싫었다.

#### 🍿 What & How
- 기존 템플릿이 있더라도 쉽게 가져가서 쓸 수 있어야 한다.
  - django-admin startpeoject의 --template 을 활용하여 해당 템플릿을 쉽게 활용할 수 있게 하자.
- 조금 더 개선할 여지가 있지 않을까?
  - dockerize 등 기타 요소도 추가하여 만들자 -> [dpd_template](https://github.com/shinkeonkim/dpd_template)
  - 이것도 너무 예전에 만든 것 같아서 최신화가 필요하다.
- 사용자가 shell에서 더 설정하는 식으로 할 수 없을까?

</details>

### [drawing, 간단 그림판](https://github.com/shinkeonkim/drawing)

- 흰 화면에서 간단한 그림을 그리자.
- 획 크기 조절, 모두 지우기 기능 제공


<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 단지 흰 화면에서 그림을 간단하게 그리고 싶었다.
- canvas를 다루는 간단한 예제를 만들고 싶었다.

#### 🍿 What & How
- 색깔을 더 추가해도 될 것 같다.
- 아이패드/휴대폰 등에서 터치 이벤트가 추가되어도 좋을 것 같다.

</details>


</div>

<div id="paused-projects">

## Paused

### [wordle-online](https://github.com/shinkeonkim/wordle-online)

- wordle 게임을 온라인에서 여러명이 같이 하는 방법이 없을까?

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- wordle 게임을 혼자 하다가, 뭔가 다같이 하는 사이트를 만드는 겸, websocket을 써볼 수 있지 않을까 해서 만들어볼까 한 프로젝트

#### 🍿 What & How
- 진행중에 시간이 부족해 포기하고 있었음.. 이후 다시 간단하게 시도해볼 예정

</details>

### [notion-blog, 노션을 활용한 블로그](https://github.com/shinkeonkim/notion-blog)

- 노션 정보를 가져와, React.js 상에서 커스텀을 추가해보자

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 블로그를 여러 곳에서 한번 써보자는 생각으로 만들어봤다.

#### 🍿 What & How
- react-notion-x 패키지를 사용하면 쉽게 할 수 있었다. 하지만 생각보다 기존 블로그에 비해 이점이 크게 느껴지지 않아 중단했다.

</details>


### [1day1commit](https://github.com/shinkeonkim/1day1commit)

- 1일 1커밋을 하지 않은 날에 알림이 오게 하는 앱을 만들자

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 1일 1커밋에 미쳐있던 시기가 있었다.

#### 🍿 What & How
- Expo를 통해 앱을 만들고 별도 서버에서 1일 1커밋을 꾸준히 체킹하는 식으로 하고 싶었다.
- 하지만 1일 1커밋을 이렇게까지 체크해야 하는가?와 별도 캘린더 앱을 통해서 체크할 수 있지 않을까 라는 생각으로 중단했다.

</details>

### [hangul, 한글 디자인 프로젝트](https://github.com/shinkeonkim/hangul)

- 한글을 소재로 인터랙티프 웹 사이트를 만들 수 있을까?

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 한글을 소재로 인터랙티프 웹 사이트를 만들 수 있을까? 라는 호기심에서 시작했다.

#### 🍿 What & How
- 첫 메인 페이지는 모든 한글의 글자가 쭈르륵 화면에 노출되면서 강조가 되면 좋겠다는 생각을 했고, 각 글자를 클릭하면 관련 글자들 페이지로 바뀌는 식을 원했다.
  - 메인 페이지를 대강 구상했지만, 예상만큼 완성도가 나오지 않아서 좀더 디자인과 웹 최적화를 공부하고 해야겠다는 생각으로 중단함.

</details>

### [can you catch circle?, 원을 잡아라](https://github.com/shinkeonkim/can-you-catch-circle)

- 원을 잡는 게임

<img src="https://user-images.githubusercontent.com/47373998/146671635-10c41ed7-fcbc-443a-ab16-1ce7f85d0391.jpg" width="200">

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 간단한 애니메이션을 이용해서 게임 요소를 만들어보고 싶었다.

#### 🍿 What & How
- 각 스테이지마다 원을 잡는 기믹이 있어야 한다.
  - 첫번째는 예시로 가만히 있는 원을 클릭하게 한다.
  - 다음 스테이지에서 원이 좌우로 움직이게 한다.
  - 그 다음 스테이지를 만들다가 중단함.

</details>

### [likelion-badge, 대학생 멋쟁이사자처럼 프로필을 이쁘게 보여주는 프로젝트](https://github.com/shinkeonkim/likelion-badge)

- 대학생 멋쟁이사자처럼 프로필을 이쁘게 보여주는 프로젝트

<img src="https://raw.githubusercontent.com/shinkeonkim/likelion-badge/e4c75f98836ad11399b3310c81063dde4972a287/svgs/shield_badge.svg" width="150">

<img src="https://raw.githubusercontent.com/shinkeonkim/likelion-badge/e4c75f98836ad11399b3310c81063dde4972a287/svgs/likelion_university_v1.svg" width="500">


<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 여타 Github README.md에 남기는 내용처럼 멋쟁이사자처럼의 프로필을 예쁘게 남기게 하고 싶었다.

#### 🍿 What & How
- 간단하게 배포하자
  - -> heroku에 배포
  - -> heroku의 유료화 정책으로 해당 프로젝트 삭제 -> 제대로 작동하지 않는 중
  - github page를 활용해서 단순한 js 로직으로 만들 수 있을지 고민 중에 중단됨.

</details>

</div>




<!--

### 

- 

<details>
<summary>
  자세한 내용 보기
</summary>

#### ❓ why
- 

#### 🍿 What & How
- 

</details>

-->







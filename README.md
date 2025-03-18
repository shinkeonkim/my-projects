# my-projects
지금까지 진행했던 프로젝트들을 정리합니다

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

## Paused

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







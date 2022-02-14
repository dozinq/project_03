# 📌 My Third Project 📋

---

##### - Outline : 2022년 2월 11일, 세번째 프로젝트를 수행하였다. 지난 프로젝트와는 달리, 이번에는 Web Project였으며, 얕고 짧은 지식을 가지고 있지만, 그것들을 총동원하여 주어진 목표에 도달하려고 많이 노력하였다. 이번 프로젝트에서는 동기들에게 많은 도움을 받았지만, 그로 인해 더 자극을 받고 앞으로 나아가고자 하는 계기가 되었음에 많은 의미가 있는 것 같다. 이 문서에서는 오늘 내가 활용한 지식들과 느낀점을 주로 서술해 보고자 한다.

---

<br>

# **< Title : " 반응형 웹 페이지 구성 *"* >**

<br>

- *요구사항 : 커뮤니티 서비스 개발을 위한 화면 구성 단계로, 유저가 보는 프론트 엔드를 개발합니다. 앞으로는 필수적으로 구현해야 하는 내용을 해결합니다.*

<br>

### - case #1. 네비게이션 바(Navigation Bar)와 푸터(Footer)의 구현

#### 🧾 Brief Explanation

- 네비게이션 바는 스크롤을 하더라도 항상 상단에 고정되어 있어야 한다.
- 로고 이미지는 주어진 이미지 파일을 사용하며, 클릭 시 해당 페이지(02_home.html)로 이동해야 한다.
- 네비게이션 바 내부의 네비게이션 리스트는 ul과 li요소를 사용하고, 오른쪽에 배치한다.
- 네비게이션 리스트의 각 항목들을 클릭 시 해당 페이지(02_home.html,  03_community.html, #)로 이동해야 한다.
- 네비게이션 리스트의 Login 항목을 클릭 시 요소가 Modal 컴포넌트를 통하여 나타나며, form 요소를 배치시켜야 한다. 또한, form요소 내부의 비밀번호는 표시되지 않는다.



#### 🔑 Solution

```html
<nav class="navbar navbar-expand-md navbar-dark bg-dark sticky-top">
```

: 네비게이션 바가 스크롤을 하더라도 항상 상단에 고정될 수 있게 'sticky-top'을 작성해 주었다.



```html
<img src="images/logo.png" alt="logo image" style="width: 120px;">
```

: 주어진 로고 이미지를 삽입하였다.



```html
<a class="navbar-brand" href="02_home.html">
```

: 로고 이미지를 클릭 가능한 링크로 설정하였고, 해당 페이지(02_home.html)로 이동할 수 있게 하였다.



```html
<div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="02_home.html">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="03_community.html">Community</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#" data-bs-toggle="modal" data-bs-target="#loginModal">Login</a>
            </li>
          </ul>
        </div>
```

: 네비게이션 바 내부의 네비게이션 리스트(Home, Community, Login)는 ul과 li요소를  사용하였고, 이전에 작성하였던 justify-conten-between으로 해당 항목은 오른쪽에 배치될 수 있게 하였다. 또한, 각 해당 페이지에 링크를 설정해 주었다.



```html
<button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
</button>
```

: 해당 가로 크기에 도달하기 전까지 버튼으로 교체되게끔 하였으며, 클릭했을 시 세부 항목을 볼 수 있도록 설정하였다.



```html
<div class="modal fade" id="loginModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="exampleModalLabel">Login</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div>
        <form class="container p-4">
          <div class="mb-3">
            <label for="exampleInputEmail1" class="form-label">Email address</label>
            <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
            <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
          </div>
          <div class="mb-3">
            <label for="exampleInputPassword1" class="form-label">Password</label>
            <input type="password" class="form-control" id="exampleInputPassword1">
          </div>
          <div class="mb-3 form-check">
            <input type="checkbox" class="form-check-input" id="exampleCheck1">
            <label class="form-check-label" for="exampleCheck1">Check me out</label>
          </div>
          <div class="modal-footer">
            <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
            <button type="submit" class="btn btn-primary">Submit</button>
          </div>
        </form>
      </div>
    </div>
  </div>
```

: 네비게이션 리스트의 Login 항목을 클릭하면 요소가 Modal 컴포넌트를 통하여 나타날 수 있도록 하였다. 또한, Modal 컴포넌트 내부에는 form요소를 배치하였고, Modal 컴포넌트에서 form요소 내부의 비밀번호는 표시되지 않도록 하였다.

<br>

### - case #2. 헤더(Header)와 섹션(Section)의 구현

#### 🧾 Brief Explanation

- Header는 Carousel 컴포넌트로 구성한다. 주어진 이미지들이 자동으로 전환되어야 한다.
- Box Office 문구는 자유롭게 스타일링한다.
- Section은 컨테이너 내부에 위치시키며, 개별 요소(article)들은 이미지, 제목, 설명을 포함하는 Card 컴포넌트로 구성하고, 일정한 간격으로 떨어트려야 합니다.

- article들은 Viewport의 가로 크기가 576px미만일 경우에는 한 행에 1개씩 표시하고, 그 이상일 때는 한 행에 2개 이상 표시한다.



#### 🔑 Solution

```html
<header>
    <div id="carouselExampleInterval" class="carousel slide" data-bs-ride="carousel">
      <div class="carousel-inner">
        <div class="carousel-item active" data-bs-interval="4000">
          <img src="images/header1.jpg" class="d-block w-100" alt="header1">
        </div>
        <div class="carousel-item" data-bs-interval="4000">
          <img src="images/header2.jpg" class="d-block w-100" alt="header2">
        </div>
        <div class="carousel-item">
          <img src="images/header3.jpg" class="d-block w-100" alt="header3">
        </div>
      </div>
      <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleInterval" data-bs-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleInterval" data-bs-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>
  </header>
```

: header는 Carousel 컴포넌트로 구성하였는데, Bootstrap에서 원하는 형식을 찾을 수 있었고 가져와서 목적에 맞게 다듬었다. data-bs-interval을 4000으로 맞춰주니 그 동안 내가 다른 페이지들에서 보았던 속도로 구현할 수 있었다.



```html
h1 class="d-flex flex-row justify-content-center mb-4 fw-bold">Boxoffice</h1>

  <section class="d-flex flex-row row">
    <article class="d-flex col-12 col-sm-6 col-lg-4">
      <div class="card">
        <img src="images/movie1.jpg" class="card-img-top" alt="The_Shawshank_Redemption_image">
        <div class="card-body">
          <h5 class="card-title text-center fw-bold">쇼생크 탈출</h5>
          <p class="card-text text-center">촉망 받던 은행 부지점장 앤디는 아내와 그 애인을 살해한 혐의로 종신형을 받고 쇼생크 교도소에 수감되는데..</p>
        </div>
      </div>
    </article>
    <article class="d-flex col-12 col-sm-6 col-lg-4">
      <div class="card">
        <img src="images/movie2.jpg" class="card-img-top" alt="Dead_Poets_Society_image">
        <div class="card-body">
          <h5 class="card-title text-center fw-bold">죽은 시인의 사회</h5>
          <p class="card-text text-center">미국 입시 명문고 웰튼 아카데미, 키팅은 공부가 인생의 전부인 학생들이 아이비리그로 가기 위해 고군분투하는 그 곳에 영어 교사로 부임하게 되는데..</p>
        </div>
      </div>
    </article>
    <article class="d-flex col-12 col-sm-6 col-lg-4">
      <div class="card">
        <img src="images/movie3.jpg" class="card-img-top" alt="The_Dark_Knight_Rises">
        <div class="card-body">
          <h5 class="card-title text-center fw-bold">다크 나이트 라이즈</h5>
          <p class="card-text text-center">범죄방지 덴트법으로 인해 한동안 평화가 지속되던 고담시에 마스크를 쓴 잔인한 악당들이 파멸을 예고하며 나타나는데..</p>
        </div>
      </div>
    </article>
    <article class="d-flex col-12 col-sm-6 col-lg-4">
      <div class="card">
        <img src="images/movie4.jpg" class="card-img-top" alt="The_Grand_Budapest_Hotel">
        <div class="card-body">
          <h5 class="card-title text-center fw-bold">그랜드 부다페스트 호텔</h5>
          <p class="card-text text-center">어느 날, 세계 최고의 부호 마담 D.가 의문의 살인을 당한다. 전설적인 호텔 지배인이자 그녀의 연인인 구스타브는 유력한 용의자로 지목받게 되는데.. </p>
        </div>
      </div>
    </article>
    <article class="d-flex col-12 col-sm-6 col-lg-4">
      <div class="card">
        <img src="images/movie5.jpg" class="card-img-top" alt="Her">
        <div class="card-body">
          <h5 class="card-title text-center fw-bold">그녀</h5>
          <p class="card-text text-center">다른 사람의 편지를 써주는 대필 작가로 일하고 있는 테오도르는 정작 자신은 아내와 별거 중인 채 외롭고 공허한 삶을 살아가고 있는데..</p>
        </div>
      </div>
    </article>
    <article class="d-flex col-12 col-sm-6 col-lg-4">
      <div class="card">
        <img src="images/movie6.jpg" class="card-img-top" alt="The_Greatest_Showman">
        <div class="card-body">
          <h5 class="card-title text-center fw-bold">위대한 쇼맨</h5>
          <p class="card-text text-center">쇼 비즈니스의 창시자이자, 꿈의 무대로 전세계를 매료시킨 남자 ‘바넘’의 이야기에서 영감을 받아 탄생한 오리지널 뮤지컬 영화!</p>
        </div>
      </div>
    </article>
  </section>
```

: 섹션부분은 그동안 배웠던 breakpoint를 잘 활용하여 페이지가 늘어나고 줄어듦에 따라 다르게 표현되어 질 수 있도록 표시해주었으며, 각 card의 구성은 영화정보를 찾아서 표시할 수 있었고, 이것을 구현할 때가 가장 즐거웠고 희망을 얻을 수 있었던 것 같다.

<br>

### - case #3. Community항목의 구현

#### 🧾 Brief Explanation

- Community 페이지는 크게 게시판 목록, 게시판으로 이루어져 있고, 모두 div.main 요소로 둘러 쌓여 있다.
- 게시판 목록과 게시판, 게시글 페이징은 모두 컨테이너 내부에 위치시킨다.
- 게시판 목록은 aside 요소로 이루어져 있어야 하고, 내부의 각 항목은 List group 컴포넌트를 활용한다.
- 게시판 목록 내부의 각 항목은 클릭이 가능한 링크로 만든다.
- Viewport의 가로 크기가 992px 이상일 경우에는 게시판 목록 내부의 항목은 div.main영역의 내부에서 좌측 1/6 만큼의 너비를 가지고, 992px 미만일 경우에는 div.main영역의 내부에서 전체만큼의 너비를 가진다.
- Viewport의 가로 크기가 992px 이상일 경우에는 게시글이 표(table) 요소로  표시되며, div.main영역의 내부에서 우측 5/6 만큼의 너비를 가지고, 992px 미만일 경우에는 게시글이 글(article) 요소들의 집합으로 표시되고 가로선으로 구분시키고 div.main영역의 내부에서 전체만큼의 너비를 가집니다.
- 게시글은 글 제목, 영화 제목, 사용자 id, 작성시간으로 구성되어 있다.
- 게시글 페이징(paginator)은 게시판 아래에 위치시키고, 자신의 영역 안에서 좌우 중앙 정렬되어 있습니다. 내부의 요소들은 클릭이 가능한 링크로 만듭니다.



#### 🔑 Solution

```html
<div class="main container">
    <h1 class="text-center fw-bold my-5">Community</h1>

    <!-- Sidebar -->
    <div class="row">
      <aside class="col-12 col-lg-2">
        <ul class="list-unstyled">
          <li class="p-3 border"><a class="text-decoration-none" href="#">Boxoffice</a></li>
          <li class="p-3 border"><a class="text-decoration-none" href="#">Movies</a></li>
          <li class="p-3 border"><a class="text-decoration-none" href="#">Genres</a></li>
          <li class="p-3 border"><a class="text-decoration-none" href="#">Actors</a></li>
        </ul>
      </aside>
```

: aside요소로 이루어진 게시판 목록을 생성하였다. 각 항목은 list group 컴포넌트를 활용하였다.



```html
 <!-- Board -->
      <section class="col-10 col-lg-10">
        <!-- Table View -->
        <div class="d-none d-lg-block">
          <table class="table">
            <thead class="bg-dark text-white fw-bold">
              <tr>
                <th scope="col">영화 제목</th>
                <th scope="col">글 제목</th>
                <th scope="col">작성자</th>
                <th scope="col">작성 시간</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <th scope="row">Great Movie title</th>
                <td>Best Movie Ever</td>
                <td>user</td>
                <td>1 minute ago</td>
              </tr>
              <tr>
                <th scope="row">Great Movie title</th>
                <td>Movie Test</td>
                <td>user</td>
                <td>1 minute ago</td>
              </tr>
              <tr>
                <th scope="row">Great Movie title</th>
                <td>Movie Test</td>
                <td>user</td>
                <td>1 minute ago</td>
              </tr>
              <tr>
                <th scope="row">Great Movie title</th>
                <td>Movie Test</td>
                <td>user</td>
                <td>1 minute ago</td>
              </tr>
              <tr>
                <th scope="row">Great Movie title</th>
                <td>Movie Test</td>
                <td>user</td>
                <td>1 minute ago</td>
              </tr>
              <tr>
                <th scope="row">Great Movie title</th>
                <td>Movie Test</td>
                <td>user</td>
                <td>1 minute ago</td>
              </tr>
              <tr>
                <th scope="row">Great Movie title</th>
                <td>Movie Test</td>
                <td>user</td>
                <td>1 minute ago</td>
              </tr>
            </tbody>
          </table>
        </div>
```

: 게시판은 가로크기에 따라 달라지게끔 하였는데, 위의 코드는 lg breakpoint를 초과할때에만 표시될 수 있는 표를 구현해주었다. dib.main영역의 내부에서 우측 5/6 만큼의 너비를 가질 수 있도록 설정해 놓았다.



```html
<!-- change table view -->
        <div class="d-block d-lg-none">
          <article>
            <hr>
            <div class="d-flex justify-content-between align-items-center">
              <h2>Best Movie Ever</h2>
              <p class="mb-0">user</p>
            </div>
            <h4>Great Movie Title</h4>
            <p>1 minute ago</p>
          </article>
          <article>
            <hr>
            <div class="d-flex justify-content-between align-items-center">
              <h2>Movie Test</h2>
              <p class="mb-0">user</p>
            </div>
            <h4>Great Movie Title</h4>
            <p>1 minute ago</p>
          </article>
          <article>
            <hr>
            <div class="d-flex justify-content-between align-items-center">
              <h2>Movie Test</h2>
              <p class="mb-0">user</p>
            </div>
            <h4>Great Movie Title</h4>
            <p>1 minute ago</p>
          </article>
        </div>
```

: 가로크기가 lg break를 초과하지 않을 때에만 위의 코드가 구현될 수 있게 설정해 놓았다. 게시글이 article요소들의 집합으로 표시되고 가로선으로 구분될수 있게 하였다. 또한, div.main영역의 내부에서 전체만큼의 너비를 가질 수 있도록 구현하였다.

<br>

## Outro

> Web과목은 더 적응해야 할 필요가 있다고 생각한다. 또한, 가지고 있는 지식뿐만 아니라 Bootstrap이나 여러 사이트를 응용해야 하는 노련함까지 필요하기 때문에 연습과 반복만이 능력을 기르는 방법이지 않을까 생각된다. 그렇게 하다보면 언젠가는 이 과제도 간단하게 해결할 수 있게 되지 않을까 생각이 들었다. 이번 프로젝트를 수행하면서, 개인이 모든 것을 해결하기엔 정말 불가능에 가깝다고 생각이 들기도 하였다. 모든 것에 타인의 도움을 기대한다는 것은 심각한 문제겠지만, 개발자에게 협동심이란 떼어낼 수 없다는 것을 다시 새롭게 느꼈던 것 같다.
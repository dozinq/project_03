# ๐ My Third Project ๐

---

##### - Outline : 2022๋ 2์ 11์ผ, ์ธ๋ฒ์งธ ํ๋ก์ ํธ๋ฅผ ์ํํ์๋ค. ์ง๋ ํ๋ก์ ํธ์๋ ๋ฌ๋ฆฌ, ์ด๋ฒ์๋ Web Project์์ผ๋ฉฐ, ์๊ณ  ์งง์ ์ง์์ ๊ฐ์ง๊ณ  ์์ง๋ง, ๊ทธ๊ฒ๋ค์ ์ด๋์ํ์ฌ ์ฃผ์ด์ง ๋ชฉํ์ ๋๋ฌํ๋ ค๊ณ  ๋ง์ด ๋ธ๋ ฅํ์๋ค. ์ด๋ฒ ํ๋ก์ ํธ์์๋ ๋๊ธฐ๋ค์๊ฒ ๋ง์ ๋์์ ๋ฐ์์ง๋ง, ๊ทธ๋ก ์ธํด ๋ ์๊ทน์ ๋ฐ๊ณ  ์์ผ๋ก ๋์๊ฐ๊ณ ์ ํ๋ ๊ณ๊ธฐ๊ฐ ๋์์์ ๋ง์ ์๋ฏธ๊ฐ ์๋ ๊ฒ ๊ฐ๋ค. ์ด ๋ฌธ์์์๋ ์ค๋ ๋ด๊ฐ ํ์ฉํ ์ง์๋ค๊ณผ ๋๋์ ์ ์ฃผ๋ก ์์ ํด ๋ณด๊ณ ์ ํ๋ค.

---

<br>

# **< Title : " ๋ฐ์ํ ์น ํ์ด์ง ๊ตฌ์ฑ *"* >**

<br>

- *์๊ตฌ์ฌํญ : ์ปค๋ฎค๋ํฐ ์๋น์ค ๊ฐ๋ฐ์ ์ํ ํ๋ฉด ๊ตฌ์ฑ ๋จ๊ณ๋ก, ์ ์ ๊ฐ ๋ณด๋ ํ๋ก ํธ ์๋๋ฅผ ๊ฐ๋ฐํฉ๋๋ค. ์์ผ๋ก๋ ํ์์ ์ผ๋ก ๊ตฌํํด์ผ ํ๋ ๋ด์ฉ์ ํด๊ฒฐํฉ๋๋ค.*

<br>

### - case #1. ๋ค๋น๊ฒ์ด์ ๋ฐ(Navigation Bar)์ ํธํฐ(Footer)์ ๊ตฌํ

#### ๐งพ Brief Explanation

- ๋ค๋น๊ฒ์ด์ ๋ฐ๋ ์คํฌ๋กค์ ํ๋๋ผ๋ ํญ์ ์๋จ์ ๊ณ ์ ๋์ด ์์ด์ผ ํ๋ค.
- ๋ก๊ณ  ์ด๋ฏธ์ง๋ ์ฃผ์ด์ง ์ด๋ฏธ์ง ํ์ผ์ ์ฌ์ฉํ๋ฉฐ, ํด๋ฆญ ์ ํด๋น ํ์ด์ง(02_home.html)๋ก ์ด๋ํด์ผ ํ๋ค.
- ๋ค๋น๊ฒ์ด์ ๋ฐ ๋ด๋ถ์ ๋ค๋น๊ฒ์ด์ ๋ฆฌ์คํธ๋ ul๊ณผ li์์๋ฅผ ์ฌ์ฉํ๊ณ , ์ค๋ฅธ์ชฝ์ ๋ฐฐ์นํ๋ค.
- ๋ค๋น๊ฒ์ด์ ๋ฆฌ์คํธ์ ๊ฐ ํญ๋ชฉ๋ค์ ํด๋ฆญ ์ ํด๋น ํ์ด์ง(02_home.html,  03_community.html, #)๋ก ์ด๋ํด์ผ ํ๋ค.
- ๋ค๋น๊ฒ์ด์ ๋ฆฌ์คํธ์ Login ํญ๋ชฉ์ ํด๋ฆญ ์ ์์๊ฐ Modal ์ปดํฌ๋ํธ๋ฅผ ํตํ์ฌ ๋ํ๋๋ฉฐ, form ์์๋ฅผ ๋ฐฐ์น์์ผ์ผ ํ๋ค. ๋ํ, form์์ ๋ด๋ถ์ ๋น๋ฐ๋ฒํธ๋ ํ์๋์ง ์๋๋ค.



#### ๐ Solution

```html
<nav class="navbar navbar-expand-md navbar-dark bg-dark sticky-top">
```

: ๋ค๋น๊ฒ์ด์ ๋ฐ๊ฐ ์คํฌ๋กค์ ํ๋๋ผ๋ ํญ์ ์๋จ์ ๊ณ ์ ๋  ์ ์๊ฒ 'sticky-top'์ ์์ฑํด ์ฃผ์๋ค.



```html
<img src="images/logo.png" alt="logo image" style="width: 120px;">
```

: ์ฃผ์ด์ง ๋ก๊ณ  ์ด๋ฏธ์ง๋ฅผ ์ฝ์ํ์๋ค.



```html
<a class="navbar-brand" href="02_home.html">
```

: ๋ก๊ณ  ์ด๋ฏธ์ง๋ฅผ ํด๋ฆญ ๊ฐ๋ฅํ ๋งํฌ๋ก ์ค์ ํ์๊ณ , ํด๋น ํ์ด์ง(02_home.html)๋ก ์ด๋ํ  ์ ์๊ฒ ํ์๋ค.



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

: ๋ค๋น๊ฒ์ด์ ๋ฐ ๋ด๋ถ์ ๋ค๋น๊ฒ์ด์ ๋ฆฌ์คํธ(Home, Community, Login)๋ ul๊ณผ li์์๋ฅผ  ์ฌ์ฉํ์๊ณ , ์ด์ ์ ์์ฑํ์๋ justify-conten-between์ผ๋ก ํด๋น ํญ๋ชฉ์ ์ค๋ฅธ์ชฝ์ ๋ฐฐ์น๋  ์ ์๊ฒ ํ์๋ค. ๋ํ, ๊ฐ ํด๋น ํ์ด์ง์ ๋งํฌ๋ฅผ ์ค์ ํด ์ฃผ์๋ค.



```html
<button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
</button>
```

: ํด๋น ๊ฐ๋ก ํฌ๊ธฐ์ ๋๋ฌํ๊ธฐ ์ ๊น์ง ๋ฒํผ์ผ๋ก ๊ต์ฒด๋๊ฒ๋ ํ์์ผ๋ฉฐ, ํด๋ฆญํ์ ์ ์ธ๋ถ ํญ๋ชฉ์ ๋ณผ ์ ์๋๋ก ์ค์ ํ์๋ค.



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

: ๋ค๋น๊ฒ์ด์ ๋ฆฌ์คํธ์ Login ํญ๋ชฉ์ ํด๋ฆญํ๋ฉด ์์๊ฐ Modal ์ปดํฌ๋ํธ๋ฅผ ํตํ์ฌ ๋ํ๋  ์ ์๋๋ก ํ์๋ค. ๋ํ, Modal ์ปดํฌ๋ํธ ๋ด๋ถ์๋ form์์๋ฅผ ๋ฐฐ์นํ์๊ณ , Modal ์ปดํฌ๋ํธ์์ form์์ ๋ด๋ถ์ ๋น๋ฐ๋ฒํธ๋ ํ์๋์ง ์๋๋ก ํ์๋ค.

<br>

### - case #2. ํค๋(Header)์ ์น์(Section)์ ๊ตฌํ

#### ๐งพ Brief Explanation

- Header๋ Carousel ์ปดํฌ๋ํธ๋ก ๊ตฌ์ฑํ๋ค. ์ฃผ์ด์ง ์ด๋ฏธ์ง๋ค์ด ์๋์ผ๋ก ์ ํ๋์ด์ผ ํ๋ค.
- Box Office ๋ฌธ๊ตฌ๋ ์์ ๋กญ๊ฒ ์คํ์ผ๋งํ๋ค.
- Section์ ์ปจํ์ด๋ ๋ด๋ถ์ ์์น์ํค๋ฉฐ, ๊ฐ๋ณ ์์(article)๋ค์ ์ด๋ฏธ์ง, ์ ๋ชฉ, ์ค๋ช์ ํฌํจํ๋ Card ์ปดํฌ๋ํธ๋ก ๊ตฌ์ฑํ๊ณ , ์ผ์ ํ ๊ฐ๊ฒฉ์ผ๋ก ๋จ์ดํธ๋ ค์ผ ํฉ๋๋ค.

- article๋ค์ Viewport์ ๊ฐ๋ก ํฌ๊ธฐ๊ฐ 576px๋ฏธ๋ง์ผ ๊ฒฝ์ฐ์๋ ํ ํ์ 1๊ฐ์ฉ ํ์ํ๊ณ , ๊ทธ ์ด์์ผ ๋๋ ํ ํ์ 2๊ฐ ์ด์ ํ์ํ๋ค.



#### ๐ Solution

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

: header๋ Carousel ์ปดํฌ๋ํธ๋ก ๊ตฌ์ฑํ์๋๋ฐ, Bootstrap์์ ์ํ๋ ํ์์ ์ฐพ์ ์ ์์๊ณ  ๊ฐ์ ธ์์ ๋ชฉ์ ์ ๋ง๊ฒ ๋ค๋ฌ์๋ค. data-bs-interval์ 4000์ผ๋ก ๋ง์ถฐ์ฃผ๋ ๊ทธ ๋์ ๋ด๊ฐ ๋ค๋ฅธ ํ์ด์ง๋ค์์ ๋ณด์๋ ์๋๋ก ๊ตฌํํ  ์ ์์๋ค.



```html
h1 class="d-flex flex-row justify-content-center mb-4 fw-bold">Boxoffice</h1>

  <section class="d-flex flex-row row">
    <article class="d-flex col-12 col-sm-6 col-lg-4">
      <div class="card">
        <img src="images/movie1.jpg" class="card-img-top" alt="The_Shawshank_Redemption_image">
        <div class="card-body">
          <h5 class="card-title text-center fw-bold">์ผ์ํฌ ํ์ถ</h5>
          <p class="card-text text-center">์ด๋ง ๋ฐ๋ ์ํ ๋ถ์ง์ ์ฅ ์ค๋๋ ์๋ด์ ๊ทธ ์ ์ธ์ ์ดํดํ ํ์๋ก ์ข์ ํ์ ๋ฐ๊ณ  ์ผ์ํฌ ๊ต๋์์ ์๊ฐ๋๋๋ฐ..</p>
        </div>
      </div>
    </article>
    <article class="d-flex col-12 col-sm-6 col-lg-4">
      <div class="card">
        <img src="images/movie2.jpg" class="card-img-top" alt="Dead_Poets_Society_image">
        <div class="card-body">
          <h5 class="card-title text-center fw-bold">์ฃฝ์ ์์ธ์ ์ฌํ</h5>
          <p class="card-text text-center">๋ฏธ๊ตญ ์์ ๋ช๋ฌธ๊ณ  ์ฐํผ ์์นด๋ฐ๋ฏธ, ํคํ์ ๊ณต๋ถ๊ฐ ์ธ์์ ์ ๋ถ์ธ ํ์๋ค์ด ์์ด๋น๋ฆฌ๊ทธ๋ก ๊ฐ๊ธฐ ์ํด ๊ณ ๊ตฐ๋ถํฌํ๋ ๊ทธ ๊ณณ์ ์์ด ๊ต์ฌ๋ก ๋ถ์ํ๊ฒ ๋๋๋ฐ..</p>
        </div>
      </div>
    </article>
    <article class="d-flex col-12 col-sm-6 col-lg-4">
      <div class="card">
        <img src="images/movie3.jpg" class="card-img-top" alt="The_Dark_Knight_Rises">
        <div class="card-body">
          <h5 class="card-title text-center fw-bold">๋คํฌ ๋์ดํธ ๋ผ์ด์ฆ</h5>
          <p class="card-text text-center">๋ฒ์ฃ๋ฐฉ์ง ๋ดํธ๋ฒ์ผ๋ก ์ธํด ํ๋์ ํํ๊ฐ ์ง์๋๋ ๊ณ ๋ด์์ ๋ง์คํฌ๋ฅผ ์ด ์์ธํ ์๋น๋ค์ด ํ๋ฉธ์ ์๊ณ ํ๋ฉฐ ๋ํ๋๋๋ฐ..</p>
        </div>
      </div>
    </article>
    <article class="d-flex col-12 col-sm-6 col-lg-4">
      <div class="card">
        <img src="images/movie4.jpg" class="card-img-top" alt="The_Grand_Budapest_Hotel">
        <div class="card-body">
          <h5 class="card-title text-center fw-bold">๊ทธ๋๋ ๋ถ๋คํ์คํธ ํธํ</h5>
          <p class="card-text text-center">์ด๋ ๋ , ์ธ๊ณ ์ต๊ณ ์ ๋ถํธ ๋ง๋ด D.๊ฐ ์๋ฌธ์ ์ด์ธ์ ๋นํ๋ค. ์ ์ค์ ์ธ ํธํ ์ง๋ฐฐ์ธ์ด์ ๊ทธ๋์ ์ฐ์ธ์ธ ๊ตฌ์คํ๋ธ๋ ์ ๋ ฅํ ์ฉ์์๋ก ์ง๋ชฉ๋ฐ๊ฒ ๋๋๋ฐ.. </p>
        </div>
      </div>
    </article>
    <article class="d-flex col-12 col-sm-6 col-lg-4">
      <div class="card">
        <img src="images/movie5.jpg" class="card-img-top" alt="Her">
        <div class="card-body">
          <h5 class="card-title text-center fw-bold">๊ทธ๋</h5>
          <p class="card-text text-center">๋ค๋ฅธ ์ฌ๋์ ํธ์ง๋ฅผ ์จ์ฃผ๋ ๋ํ ์๊ฐ๋ก ์ผํ๊ณ  ์๋ ํ์ค๋๋ฅด๋ ์ ์ ์์ ์ ์๋ด์ ๋ณ๊ฑฐ ์ค์ธ ์ฑ ์ธ๋กญ๊ณ  ๊ณตํํ ์ถ์ ์ด์๊ฐ๊ณ  ์๋๋ฐ..</p>
        </div>
      </div>
    </article>
    <article class="d-flex col-12 col-sm-6 col-lg-4">
      <div class="card">
        <img src="images/movie6.jpg" class="card-img-top" alt="The_Greatest_Showman">
        <div class="card-body">
          <h5 class="card-title text-center fw-bold">์๋ํ ์ผ๋งจ</h5>
          <p class="card-text text-center">์ผ ๋น์ฆ๋์ค์ ์ฐฝ์์์ด์, ๊ฟ์ ๋ฌด๋๋ก ์ ์ธ๊ณ๋ฅผ ๋งค๋ฃ์ํจ ๋จ์ โ๋ฐ๋โ์ ์ด์ผ๊ธฐ์์ ์๊ฐ์ ๋ฐ์ ํ์ํ ์ค๋ฆฌ์ง๋ ๋ฎค์ง์ปฌ ์ํ!</p>
        </div>
      </div>
    </article>
  </section>
```

: ์น์๋ถ๋ถ์ ๊ทธ๋์ ๋ฐฐ์ ๋ breakpoint๋ฅผ ์ ํ์ฉํ์ฌ ํ์ด์ง๊ฐ ๋์ด๋๊ณ  ์ค์ด๋ฆ์ ๋ฐ๋ผ ๋ค๋ฅด๊ฒ ํํ๋์ด ์ง ์ ์๋๋ก ํ์ํด์ฃผ์์ผ๋ฉฐ, ๊ฐ card์ ๊ตฌ์ฑ์ ์ํ์ ๋ณด๋ฅผ ์ฐพ์์ ํ์ํ  ์ ์์๊ณ , ์ด๊ฒ์ ๊ตฌํํ  ๋๊ฐ ๊ฐ์ฅ ์ฆ๊ฑฐ์ ๊ณ  ํฌ๋ง์ ์ป์ ์ ์์๋ ๊ฒ ๊ฐ๋ค.

<br>

### - case #3. Communityํญ๋ชฉ์ ๊ตฌํ

#### ๐งพ Brief Explanation

- Community ํ์ด์ง๋ ํฌ๊ฒ ๊ฒ์ํ ๋ชฉ๋ก, ๊ฒ์ํ์ผ๋ก ์ด๋ฃจ์ด์ ธ ์๊ณ , ๋ชจ๋ div.main ์์๋ก ๋๋ฌ ์์ฌ ์๋ค.
- ๊ฒ์ํ ๋ชฉ๋ก๊ณผ ๊ฒ์ํ, ๊ฒ์๊ธ ํ์ด์ง์ ๋ชจ๋ ์ปจํ์ด๋ ๋ด๋ถ์ ์์น์ํจ๋ค.
- ๊ฒ์ํ ๋ชฉ๋ก์ aside ์์๋ก ์ด๋ฃจ์ด์ ธ ์์ด์ผ ํ๊ณ , ๋ด๋ถ์ ๊ฐ ํญ๋ชฉ์ List group ์ปดํฌ๋ํธ๋ฅผ ํ์ฉํ๋ค.
- ๊ฒ์ํ ๋ชฉ๋ก ๋ด๋ถ์ ๊ฐ ํญ๋ชฉ์ ํด๋ฆญ์ด ๊ฐ๋ฅํ ๋งํฌ๋ก ๋ง๋ ๋ค.
- Viewport์ ๊ฐ๋ก ํฌ๊ธฐ๊ฐ 992px ์ด์์ผ ๊ฒฝ์ฐ์๋ ๊ฒ์ํ ๋ชฉ๋ก ๋ด๋ถ์ ํญ๋ชฉ์ div.main์์ญ์ ๋ด๋ถ์์ ์ข์ธก 1/6 ๋งํผ์ ๋๋น๋ฅผ ๊ฐ์ง๊ณ , 992px ๋ฏธ๋ง์ผ ๊ฒฝ์ฐ์๋ div.main์์ญ์ ๋ด๋ถ์์ ์ ์ฒด๋งํผ์ ๋๋น๋ฅผ ๊ฐ์ง๋ค.
- Viewport์ ๊ฐ๋ก ํฌ๊ธฐ๊ฐ 992px ์ด์์ผ ๊ฒฝ์ฐ์๋ ๊ฒ์๊ธ์ด ํ(table) ์์๋ก  ํ์๋๋ฉฐ, div.main์์ญ์ ๋ด๋ถ์์ ์ฐ์ธก 5/6 ๋งํผ์ ๋๋น๋ฅผ ๊ฐ์ง๊ณ , 992px ๋ฏธ๋ง์ผ ๊ฒฝ์ฐ์๋ ๊ฒ์๊ธ์ด ๊ธ(article) ์์๋ค์ ์งํฉ์ผ๋ก ํ์๋๊ณ  ๊ฐ๋ก์ ์ผ๋ก ๊ตฌ๋ถ์ํค๊ณ  div.main์์ญ์ ๋ด๋ถ์์ ์ ์ฒด๋งํผ์ ๋๋น๋ฅผ ๊ฐ์ง๋๋ค.
- ๊ฒ์๊ธ์ ๊ธ ์ ๋ชฉ, ์ํ ์ ๋ชฉ, ์ฌ์ฉ์ id, ์์ฑ์๊ฐ์ผ๋ก ๊ตฌ์ฑ๋์ด ์๋ค.
- ๊ฒ์๊ธ ํ์ด์ง(paginator)์ ๊ฒ์ํ ์๋์ ์์น์ํค๊ณ , ์์ ์ ์์ญ ์์์ ์ข์ฐ ์ค์ ์ ๋ ฌ๋์ด ์์ต๋๋ค. ๋ด๋ถ์ ์์๋ค์ ํด๋ฆญ์ด ๊ฐ๋ฅํ ๋งํฌ๋ก ๋ง๋ญ๋๋ค.



#### ๐ Solution

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

: aside์์๋ก ์ด๋ฃจ์ด์ง ๊ฒ์ํ ๋ชฉ๋ก์ ์์ฑํ์๋ค. ๊ฐ ํญ๋ชฉ์ list group ์ปดํฌ๋ํธ๋ฅผ ํ์ฉํ์๋ค.



```html
 <!-- Board -->
      <section class="col-10 col-lg-10">
        <!-- Table View -->
        <div class="d-none d-lg-block">
          <table class="table">
            <thead class="bg-dark text-white fw-bold">
              <tr>
                <th scope="col">์ํ ์ ๋ชฉ</th>
                <th scope="col">๊ธ ์ ๋ชฉ</th>
                <th scope="col">์์ฑ์</th>
                <th scope="col">์์ฑ ์๊ฐ</th>
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

: ๊ฒ์ํ์ ๊ฐ๋กํฌ๊ธฐ์ ๋ฐ๋ผ ๋ฌ๋ผ์ง๊ฒ๋ ํ์๋๋ฐ, ์์ ์ฝ๋๋ lg breakpoint๋ฅผ ์ด๊ณผํ ๋์๋ง ํ์๋  ์ ์๋ ํ๋ฅผ ๊ตฌํํด์ฃผ์๋ค. dib.main์์ญ์ ๋ด๋ถ์์ ์ฐ์ธก 5/6 ๋งํผ์ ๋๋น๋ฅผ ๊ฐ์ง ์ ์๋๋ก ์ค์ ํด ๋์๋ค.



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

: ๊ฐ๋กํฌ๊ธฐ๊ฐ lg break๋ฅผ ์ด๊ณผํ์ง ์์ ๋์๋ง ์์ ์ฝ๋๊ฐ ๊ตฌํ๋  ์ ์๊ฒ ์ค์ ํด ๋์๋ค. ๊ฒ์๊ธ์ด article์์๋ค์ ์งํฉ์ผ๋ก ํ์๋๊ณ  ๊ฐ๋ก์ ์ผ๋ก ๊ตฌ๋ถ๋ ์ ์๊ฒ ํ์๋ค. ๋ํ, div.main์์ญ์ ๋ด๋ถ์์ ์ ์ฒด๋งํผ์ ๋๋น๋ฅผ ๊ฐ์ง ์ ์๋๋ก ๊ตฌํํ์๋ค.

<br>

## Outro

> Web๊ณผ๋ชฉ์ ๋ ์ ์ํด์ผ ํ  ํ์๊ฐ ์๋ค๊ณ  ์๊ฐํ๋ค. ๋ํ, ๊ฐ์ง๊ณ  ์๋ ์ง์๋ฟ๋ง ์๋๋ผ Bootstrap์ด๋ ์ฌ๋ฌ ์ฌ์ดํธ๋ฅผ ์์ฉํด์ผ ํ๋ ๋ธ๋ จํจ๊น์ง ํ์ํ๊ธฐ ๋๋ฌธ์ ์ฐ์ต๊ณผ ๋ฐ๋ณต๋ง์ด ๋ฅ๋ ฅ์ ๊ธฐ๋ฅด๋ ๋ฐฉ๋ฒ์ด์ง ์์๊น ์๊ฐ๋๋ค. ๊ทธ๋ ๊ฒ ํ๋ค๋ณด๋ฉด ์ธ์  ๊ฐ๋ ์ด ๊ณผ์ ๋ ๊ฐ๋จํ๊ฒ ํด๊ฒฐํ  ์ ์๊ฒ ๋์ง ์์๊น ์๊ฐ์ด ๋ค์๋ค. ์ด๋ฒ ํ๋ก์ ํธ๋ฅผ ์ํํ๋ฉด์, ๊ฐ์ธ์ด ๋ชจ๋  ๊ฒ์ ํด๊ฒฐํ๊ธฐ์ ์ ๋ง ๋ถ๊ฐ๋ฅ์ ๊ฐ๊น๋ค๊ณ  ์๊ฐ์ด ๋ค๊ธฐ๋ ํ์๋ค. ๋ชจ๋  ๊ฒ์ ํ์ธ์ ๋์์ ๊ธฐ๋ํ๋ค๋ ๊ฒ์ ์ฌ๊ฐํ ๋ฌธ์ ๊ฒ ์ง๋ง, ๊ฐ๋ฐ์์๊ฒ ํ๋์ฌ์ด๋ ๋ผ์ด๋ผ ์ ์๋ค๋ ๊ฒ์ ๋ค์ ์๋กญ๊ฒ ๋๊ผ๋ ๊ฒ ๊ฐ๋ค.
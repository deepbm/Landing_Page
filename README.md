  # Introduction
  반응형 랜딩 페이지 제작

  <br />

  # Stack
  - HTML5
  - CSS3
  - fontawesome

  <br />

  # 구현 기능
  - 반응형 웹 페이지 구현
  - fontawesome 웹 폰트 아이콘 활용
  - 이미지에 마우스를 올리면 이미지가 줄어드는 애니메이션 기능 구현


  <br />

  # > 기억하고 싶은 코드
  - 그라디언트 배경색
    ```css
    .jumbotron {
      background: linear-gradient(to bottom, 시작 색깔, 종료 색깔);
    }
    ```
  
  - 마진 상쇄 현상을 방지하기 위해 최상위 div 박스에 padding 값을 줌

  - jumbotron-text 요소와 jumbotron-img 요소 둘 다 float 속성을 부여해야 한 행에 좌우 정렬이 된다.
    ```css
    .jumbotron-text {
      float: left;
    }
    .jumbotron-img {
      float: right;
    }
    ```
  
  - 동그란 icon 만들기
    ```html
    <i class="fas fa-mobile-alt icon"></i>
    ```
    ```css
    .icon {
      width: 100px;
      height: 100px; 
      border-radius: 50%;
      background-color: white;
      padding-top: 20px;  /* 가운데로 올 수 있게 적절하게 지정 */
    }
    ```
  
  - background-image 속성은 여러 개의 이미지를 지정할 수 있다. 이를 통해 이미지를 어둡게 표현해 낼 수 있다.
    ```css
    img {
      background-image: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url(image.png);
    }
    ```
  
  - border 속성으로 이미지가 줄어드는 애니메이션 기능 구현
    ```html
    <div class="img">
      <div class="white-box"></div>
    </div>
    ```
    ```css
    .img {
      position: relative;
    }

    .white-box {
      position: absolute;
      z-index: 5;
      width: 100%;
      height: 100%;
      border: 0px solid white;
      transition: border 0.3s;
    }

    .white-box:hover {
      border: 20px solid white;
    }
    ```

  <br />

  # Reference
  해당 프로젝트는 코딩애플 강좌 프로그램에 있는 실습 과제입니다.
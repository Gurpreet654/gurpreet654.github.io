# my_web
<!DOCTYPE html>
<html>

<head>
  <!-- Basic -->
  <meta charset="utf-8" />
  <meta http-equiv="X-UA-Compatible" content="IE=edge" />
  <!-- Mobile Metas -->
  <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no" />
  <!-- Site Metas -->
  <meta name="keywords" content="" />
  <meta name="description" content="" />
  <meta name="author" content="" />

  <title>Drool</title>

  <!-- bootstrap core css -->
  
  <!-- fonts style -->
  <!-- Custom styles for this template -->
  <!-- responsive style -->
  <link rel="stylesheet" type="text/css" href="{{ url_for('static', filename='css/styles.css') }}">
  
</head>
    <style>
        body {
            background-image: url("/static/hero-bg.jpg");
            /* Additional background properties */
        }
    </style>

<body>
  <div class="hero_area ">
    <!-- header section strats -->
    <header class="header_section">
      <div class="container-fluid">
        <nav class="navbar navbar-expand-lg custom_nav-container">
          <a class="navbar-brand" href="index.html">
            <img src="{{ url_for('static', filename='slider-img.png') }}" alt="My Image">
          </a>
          <div class="" id="">
            <div class="User_option">
              <form class="form-inline my-2  mb-3 mb-lg-0">
                <input type="search" placeholder="Search">
                <button class="btn   my-sm-0 nav_search-btn" type="submit"></button>
              </form>
            </div>

            <div class="custom_menu-btn">
              <button onclick="openNav()">
                <span class="s-1">

                </span>
                <span class="s-2">

                </span>
                <span class="s-3">

                </span>
              </button>
            </div>
            <div id="myNav" class="overlay">
              <div class="overlay-content">
                <a href="index.html">Home</a>
                <a href="about.html">About</a>
                <a href="contact.html">Contact Us</a>
              </div>
            </div>
          </div>
        </nav>
      </div>
    </header>
    <!-- end header section -->
    <!-- slider section -->
    <section class="slider_section">
   
          <div class="carousel-item active">
            <div class="container-fluid">
              <div class="row">
                <div class="col-md-5 offset-md-1">
                  <div class="detail-box">
                    <div class="number">
                      <h5>
                        01
                      </h5>
                    </div>
                    <h1>
                      Drool <br>
                      <span>
                        Pet And Animal
                      </span>
                    </h1>
                    <p>
                      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt
                    </p>
                    <div class="btn-box">
                      <a href="" class="btn-1">
                        input
                      </a>
                      <form action="{{ url_for('predict')}}"method="post">
                      	<input type="text" name="experience" placeholder="Experience" required="required" />
                          <input type="text" name="test_score" placeholder="Test Score" required="required" />
                  		<input type="text" name="interview_score" placeholder="Interview Score" required="required" />

                          <button type="submit" class="btn btn-primary btn-block btn-large">Predict</button>
                      </form>
                      <br>
                      <br>
                      {{ prediction_text }}
                    </div>
                  </div>
                </div>
                <div class="col-md-6">
                  <div class="img-box">
                    <img src="{{ url_for('static', filename='slider-img.png') }}" alt="My Image">
                  </div>
                </div>
              </div>
            </div>
          </div>

          
         
</body>

</html>

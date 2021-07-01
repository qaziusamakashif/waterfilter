{% load static %}
<!DOCTYPE html>
{% load cart_tag %}
<html lang="en">

  <head>

    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
    <meta name="description" content="">
    <meta name="author" content="">
    <link href="https://fonts.googleapis.com/css?family=Poppins:100,200,300,400,500,600,700,800,900&display=swap" rel="stylesheet">

    <title>SERVEEA.com | SERVE YOU WITH PURE WATER</title>

    <!-- Bootstrap core CSS -->
    <link href="{% static 'accounts/vendor/bootstrap/css/bootstrap.min.css' %}" rel="stylesheet">

    <!-- Additional CSS Files -->
    <link rel="stylesheet" href="{% static 'accounts/assets/css/fontawesome.css' %}">
    <link rel="stylesheet" href="{% static 'accounts/assets/css/style.css' %}">
    <link rel="stylesheet" href="{% static 'accounts/assets/css/owl.css' %}">
  </head>

  <body>

    <!-- ***** Preloader Start ***** -->
    <div id="preloader">
        <div class="jumper">
            <div></div>
            <div></div>
            <div></div>
        </div>
    </div>  
    <!-- ***** Preloader End ***** -->

    <!-- Header -->
    <div class="sub-header">
      <div class="container">
        <div class="row">
          <div class="col-md-8 col-xs-12">
            <ul class="left-info">
              <li><a href="#"><i class="fa fa-envelope"></i>contact@serveea.com</a></li>
              <li><a href="#"><i class="fa fa-phone"></i>+923041709440</a></li>
	      <li><a href="#"><i class="fa fa-phone"></i>+923164855165</a></li>
            </ul>
          </div>
          <div class="col-md-4">
            <ul class="right-icons">
              <li><a href="#"><i class="fa fa-facebook"></i></a></li>
              <li><a href="#"><i class="fa fa-twitter"></i></a></li>
              <li><a href="#"><i class="fa fa-linkedin"></i></a></li>
            </ul>
          </div>
        </div>
      </div>
    </div>

    <header class="">
      <nav class="navbar navbar-expand-lg">
        <div class="container">
          <a class="navbar-brand" href="{% url 'main' %}"><h2>SERVEEA<em> Waters</em></h2></a>
          <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarResponsive">
            <ul class="navbar-nav ml-auto">
              <li class="nav-item active">
                <a class="nav-link" href="{% url 'main' %}">Home
                  <span class="sr-only">(current)</span>
                </a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="{% url 'products' %}">Products</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="{% url 'checkout' %}">Checkout</a>
              </li>
              <li class="nav-item dropdown">
                <a class="dropdown-toggle nav-link" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">About</a>
              
                <div class="dropdown-menu">
                    <a class="dropdown-item" href="{% url 'about' %}">About Us</a>
                    <a class="dropdown-item" href="{% url 'blog' %}">Blog</a>
                    <a class="dropdown-item" href="{% url 'testimonials' %}">Testimonials</a>
                    <a class="dropdown-item" href="{% url 'terms' %}">Terms</a>
                </div>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="{% url 'contact' %}">Contact Us</a>
              </li>
              <li class="nav-item dropdown">
                <a class="dropdown-toggle nav-link" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">Login</a>
              
                <div class="dropdown-menu">
                    <a class="dropdown-item" href="{% url 'loginform' %}">Login as Member</a>
                    <a class="dropdown-item" href="{% url 'adminlogin' %}">Login as admin</a>
                    <a class="dropdown-item" href="{% url 'register' %}">Register as New Member</a>
                    
                </div>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="{% url 'cart_detail' %}">Cart</a>
              </li>
            </ul>
          </div>
        </div>
      </nav>
    </header>

    <!-- Page Content -->
    <!-- Banner Starts Here -->
    <div class="main-banner header-text" id="top">
        <div class="Modern-Slider">
          <!-- Item -->
          <div class="item item-1">
            <div class="img-fill">
                <div class="text-content">
                  <h6>Another project by SERVEEA!</h6>
                  <h4>WE WELCOME YOU TO <br> SERVEEA WATERS</h4>
                  <p>We have number of quality products for you because SERVEA never compromises on health. </p>
                  <a href="{% url 'products' %}" class="filled-button">Products</a>
                </div>
            </div>
          </div>
          <!-- // Item -->
          <!-- Item -->
          <div class="item item-2">
            <div class="img-fill">
                <div class="text-content">
                  <h6>Another project by SERVEEA!</h6>
                  <h4>WE WELCOME YOU TO <br> SERVEEA WATERS</h4>
                  <p>if you want to know more about us. No issue at all just click the button below and know everything about SERVEEA WATERS</p>
                  <a href="{% url 'about' %}" class="filled-button">About Us</a>
                </div>
            </div>
          </div>
          <!-- // Item -->
          <!-- Item -->
          <div class="item item-3">
            <div class="img-fill">
                <div class="text-content">
                   <h6>Another project by SERVEEA!</h6>
                  <h4>WE WELCOME YOU TO <br> SERVEEA WATERS</h4>
                  <p>For any query and if you want to visit SERVEEA WATERS. feel free to contact us any time and visit our company anytime.</p>
                  <a href="{% url 'contact' %}" class="filled-button">Contact Us</a>
                </div>
            </div>
          </div>
          <!-- // Item -->
        </div>
    </div>
    <!-- Banner Ends Here -->

    <div class="request-form">
      <div class="container">
        <div class="row">
          <div class="col-md-8">
            <h4>Request a call back right now ?</h4>
            <span>We feel happy to answer our customers. Contact now!.</span>
          </div>
          <div class="col-md-4">
            <a href="{% url 'contact' %}" class="border-button">Contact Us</a>
          </div>
        </div>
      </div>
    </div>

    <div class="services">
      <div class="container">
       
        <div class="row">
          <div class="col-md-12">
            <div class="section-heading">
              <h2>Featured <em>Products</em></h2>
              <span>HERE ARE OUR FEATURED PRODUCTS</span>
            </div>
          </div>
          {% for data in about %}
            <div class="col-md-4">
              <div class="service-item">
                <img src={{data.image.url}}  alt="">
                <div class="down-content">
                  <h4>{{data.name}}</h4> 
                  <div style="margin-bottom:10px;">
                    <span> <del><sup>$</sup>{{data.price}}</del>  <sup>$</sup>{{data.Discount}}</span>
                  </div>

                  <p>{{data.Our_Product_Description}}</p>
                  <a href="{% url 'products_details' data.id%}" class="filled-button">View More</a>
                </div>
              </div>
              
              <br>
            </div>
          {% endfor %}
          
          
        </div>
       
      </div>
    </div>

    <div class="fun-facts">
      <div class="container">
        <div class="more-info-content">
          <div class="row">
            <div class="col-md-6">
              <div class="left-image">
                <img src="{% static 'accounts/assets/images/about-1-570x350.jpg' %}" class="img-fluid" alt="">
              </div>
            </div>
            <div class="col-md-6 align-self-center">
              <div class="right-content">
                <span>Who we are</span>
                <h2>Get to know about <em>our company</em></h2>
                <p>SERVEEA WATERS is the first company in the history of water companies who offer their customers to see live filteration of water. So they can know what exactly they are drinking!</p>
                <a href="{% url 'about' %}" class="filled-button">Read More</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="more-info">
      <div class="container">
        <div class="section-heading">
          <h2>Read our <em>Blog</em></h2>
          <span>Read Our blogs to get more information about the water and its purification</span>
        </div>

        <div class="row" id="tabs">
          <div class="col-md-4">
            <ul>
              <li><a href='#tabs-1'>Lorem ipsum dolor sit amet, consectetur adipisicing <br> <small>John Doe &nbsp;|&nbsp; 27.07.2020 10:10</small></a></li>
              <li><a href='#tabs-2'>Mauris lobortis quam id dictum dignissim <br> <small>John Doe &nbsp;|&nbsp; 27.07.2020 10:10</small></a></li>
              <li><a href='#tabs-3'>Class aptent taciti sociosqu ad litora torquent per <br> <small>John Doe &nbsp;|&nbsp; 27.07.2020 10:10</small></a></li>
            </ul>

            <br>

            <div class="text-center">
              <a href="{% url 'blog' %}" class="filled-button">Read More</a>
            </div>

            <br>
          </div>

          <div class="col-md-8">
            <section class='tabs-content'>
              <article id='tabs-1'>
                <img src="{% static 'accounts/assets/images/blog-image-1-940x460.jpg' %}" alt="">
                <h4><a href="blog-details.html">Lorem ipsum dolor sit amet, consectetur adipisicing.</a></h4>
                <p>Sed ut dolor in augue cursus ultrices. Vivamus mauris turpis, auctor vel facilisis in, tincidunt vel diam. Sed vitae scelerisque orci. Nunc non magna orci. Aliquam commodo mauris ante, quis posuere nibh vestibulum sit amet.</p>
              </article>
              <article id='tabs-2'>
                <img src="{% static 'accounts/assets/images/blog-image-2-940x460.jpg' %}" alt="">
                <h4><a href="blog-details.html">Mauris lobortis quam id dictum dignissim</a></h4>
                <p>Sed ut dolor in augue cursus ultrices. Vivamus mauris turpis, auctor vel facilisis in, tincidunt vel diam. Sed vitae scelerisque orci. Nunc non magna orci. Aliquam commodo mauris ante, quis posuere nibh vestibulum sit amet</p>
              </article>
              <article id='tabs-3'>
                <img src="{% static 'accounts/assets/images/blog-image-3-940x460.jpg' %}" alt="">
                <h4><a href="blog-details.html">Class aptent taciti sociosqu ad litora torquent per</a></h4>
                <p>Mauris lobortis quam id dictum dignissim. Donec pellentesque erat dolor, cursus dapibus turpis hendrerit quis. Suspendisse at suscipit arcu. Nulla sed erat lectus. Nulla facilisi. In sit amet neque sapien. Donec scelerisque mi at gravida efficitur. Nunc lacinia a est eu malesuada. Curabitur eleifend elit sapien, sed pulvinar orci luctus eget. 
                </p>
              </article>
            </section>
          </div>
        </div>

        
      </div>
    </div>

     <div class="testimonials">
      <div class="container">
        <div class="row">
          <div class="col-md-12">
            <div class="section-heading">
              <h2>What they say <em>about us</em></h2>
              <span>testimonials from our greatest clients</span>
            </div>
          </div>
          <div class="col-md-12">
            <div class="owl-testimonials owl-carousel">
              
              <div class="testimonial-item">
                <div class="inner-content">
                  <h4>George Walker</h4>
                  <span>Chief Financial Analyst</span>
                  <p>"I just wanted to share a quick note and let you know that you guys do a really good job. I'm glad I decided to work with you."</p>
                </div>
                <img src="..\..\static\accounts\assets\images\60x60.jpg" alt="null">
              </div>
              
              <div class="testimonial-item">
                <div class="inner-content">
                  <h4>John Smith</h4>
                  <span>Market Specialist</span>
                  <p>"First of all thanks to you for a very quick delivery. I happy to see what i ordered. Thanks again."</p>
                </div>
                <img src="..\..\static\accounts\assets\images\60x601.jpg" alt="null">
              </div>
              
              <div class="testimonial-item">
                <div class="inner-content">
                  <h4>David Wood</h4>
                  <span>Chief Accountant</span>
                  <p>"It's really great how easy your websites are to update and manage. I am very happy with your services."</p>
                </div>
                <img src="..\..\static\accounts\assets\images\60x605.jpg" alt="null">
              </div>
              
              <div class="testimonial-item">
                <div class="inner-content">
                  <h4>Andrew Boom</h4>
                  <span>Marketing Head</span>
                  <p>"Good Communication and very coporative you are. Highly recommended to all. Thanks."</p>
                </div>
                <img src="..\..\static\accounts\assets\images\60x604.jpg" alt="null">
              </div>
              
            </div>
          </div>
        </div>
      </div>
    </div>


    <div class="callback-form">
      <div class="container">
        <div class="row">
          <div class="col-md-12">
            <div class="section-heading">
              <h2>Request a <em>call back</em></h2>
              <span>We feel happy to communicate with our customers</span>
            </div>
          </div>
          <div class="col-md-12">
            <div class="contact-form">
              <form id="contact" action="" method="POST">
                {% csrf_token %}
                <div class="row">
                  <div class="col-lg-4 col-md-12 col-sm-12">
                    <fieldset>
                      <input name="name" type="text" class="form-control" id="name" placeholder="Full Name" required="">
                    </fieldset>
                  </div>
                  <div class="col-lg-4 col-md-12 col-sm-12">
                    <fieldset>
                      <input name="email" type="text" class="form-control" id="email" pattern="[^ @]*@[^ @]*" placeholder="E-Mail Address" required="">
                    </fieldset>
                  </div>
                  <div class="col-lg-4 col-md-12 col-sm-12">
                    <fieldset>
                      <input name="subject" type="text" class="form-control" id="subject" placeholder="Subject" required="">
                    </fieldset>
                  </div>
                  <div class="col-lg-12">
                    <fieldset>
                      <textarea name="message" rows="6" class="form-control" id="message" placeholder="Your Message" required=""></textarea>
                    </fieldset>
                  </div>
                  <div class="col-lg-12">
                    <fieldset>
                      <button type="submit" id="form-submit" class="border-button">Send Message</button>
                    </fieldset>
                  </div>
                </div>
              </form>
            </div>
          </div>
        </div>

        <br>
        <br>
        <br>
        <br>
      </div>
    </div>

    <!-- Footer Starts Here -->
    <footer>
      <div class="container">
        <div class="row">
          <div class="col-md-3 footer-item">
            <h4>SERVEEA WATERS</h4>
            <p>presenting you the true meaning of pureity. Because we believe in health.</p>
            <ul class="social-icons">
              <li><a rel="nofollow" href="#" target="_blank"><i class="fa fa-facebook"></i></a></li>
              <li><a href="#"><i class="fa fa-twitter"></i></a></li>
              <li><a href="#"><i class="fa fa-linkedin"></i></a></li>
            </ul>
          </div>
          <div class="col-md-3 footer-item">
            <h4>Useful Links</h4>
            <ul class="menu-list">
              <li><a href="#">Vivamus ut tellus mi</a></li>
              <li><a href="#">Nulla nec cursus elit</a></li>
              <li><a href="#">Vulputate sed nec</a></li>
              <li><a href="#">Cursus augue hasellus</a></li>
              <li><a href="#">Lacinia ac sapien</a></li>
            </ul>
          </div>
          <div class="col-md-3 footer-item">
            <h4>Additional Pages</h4>
            <ul class="menu-list">
              <li><a href="#">Products</a></li>
              <li><a href="#">About Us</a></li>
              <li><a href="#">Blog</a></li>
              <li><a href="#">Contact Us</a></li>
              <li><a href="#">Terms</a></li>
            </ul>
          </div>
          <div class="col-md-3 footer-item last-item">
            <h4>Contact Us</h4>
            <div class="contact-form">
              <form id="contact footer-contact" action="" method="post">
                <div class="row">
                  <div class="col-lg-12 col-md-12 col-sm-12">
                    <fieldset>
                      <input name="name" type="text" class="form-control" id="name" placeholder="Full Name" required="">
                    </fieldset>
                  </div>
                  <div class="col-lg-12 col-md-12 col-sm-12">
                    <fieldset>
                      <input name="email" type="text" class="form-control" id="email" pattern="[^ @]*@[^ @]*" placeholder="E-Mail Address" required="">
                    </fieldset>
                  </div>
                  <div class="col-lg-12">
                    <fieldset>
                      <textarea name="message" rows="6" class="form-control" id="message" placeholder="Your Message" required=""></textarea>
                    </fieldset>
                  </div>
                  <div class="col-lg-12">
                    <fieldset>
                      <button type="submit" id="form-submit" class="filled-button">Send Message</button>
                    </fieldset>
                  </div>
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>
    </footer>
    
    <div class="sub-footer">
      <div class="container">
        <div class="row">
          <div class="col-md-12">
            <p>
                Copyright © 2020 SERVEEA
                
            </p>
          </div>
        </div>
      </div>
    </div>

    <!-- Bootstrap core JavaScript -->
    <script src="{% static 'accounts/vendor/jquery/jquery.min.js' %}"></script>
    <script src="{% static 'accounts/vendor/bootstrap/js/bootstrap.bundle.min.js' %}"></script>

    <!-- Additional Scripts -->
    <script src="{% static 'accounts/assets/js/custom.js' %}"></script>
    <script src="{% static 'accounts/assets/js/owl.js' %}"></script>
    <script src="{% static 'accounts/assets/js/slick.js' %}"></script>
    <script src="{% static 'accounts/assets/js/accordions.js' %}"></script>

    <script language = "text/Javascript"> 
      cleared[0] = cleared[1] = cleared[2] = 0; //set a cleared flag for each field
      function clearField(t){                   //declaring the array outside of the
      if(! cleared[t.id]){                      // function makes it static and global
          cleared[t.id] = 1;  // you could use true and false, but that's more typing
          t.value='';         // with more chance of typos
          t.style.color='#fff';
          }
      }
    </script>

  </body>
</html>

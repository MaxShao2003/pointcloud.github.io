<!DOCTYPE html>
<html lang="zh">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>点云配准体验平台</title>
    <link rel="stylesheet" href="fontawesome-5.5/css/all.min.css" />
    <link rel="stylesheet" href="slick/slick.css">
    <link rel="stylesheet" href="slick/slick-theme.css">
    <link rel="stylesheet" href="magnific-popup/magnific-popup.css">
    <link rel="stylesheet" href="css/bootstrap.min.css" />
    <link rel="stylesheet" href="css/tooplate-infinite-loop.css" />
<!--
Tooplate 2117 Infinite Loop
https://www.tooplate.com/view/2117-infinite-loop
-->

  </head>
  <body>    
    <!-- Hero section -->
    <section id="infinite" class="text-white tm-font-big tm-parallax">
      <!-- Navigation -->
      <nav class="navbar navbar-expand-md tm-navbar" id="tmNav">              
        <div class="container">   
          <div class="tm-next">
              <a href="#infinite" class="navbar-brand">点云配准</a>
          </div>             
            
          <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <i class="fas fa-bars navbar-toggler-icon"></i>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav ml-auto">
              <li class="nav-item">
                  <a class="nav-link tm-nav-link" href="#infinite">主页</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link tm-nav-link" href="#whatwedo">算法介绍</a>
              </li>
              <li class="nav-item">
                <a class="nav-link tm-nav-link" href="#testimonials">数据集</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link tm-nav-link" href="#gallery">效果展示</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link tm-nav-link" href="#contact">性能指标</a>
              </li>                    
            </ul>
          </div>        
        </div>
      </nav>
      
      <div class="text-center tm-hero-text-container">
        <div class="tm-hero-text-container-inner">
            <h2 class="tm-hero-title">点云配准展示&体验平台</h2>
            <p class="tm-hero-subtitle">
              欢迎体验点云配准算法的奇妙世界！
              <br>中国大学生计算机设计大赛-算法设计与应用项目
            </p>
        </div>        
      </div>

      <div class="tm-next tm-intro-next">
        <a href="#whatwedo" class="text-center tm-down-arrow-link">
          <i class="fas fa-2x fa-arrow-down tm-down-arrow"></i>
        </a>
      </div>      
    </section>

    <section id="whatwedo" class="tm-section-pad-top">
      
      <div class="container">

            <div class="row tm-content-box"><!-- first row -->
                <div class="col-lg-12 col-xl-12">
                    <div class="tm-intro-text-container">
                        <h2 class="tm-text-primary mb-4 tm-section-title">算法介绍</h2>
                        <p class="mb-4 tm-intro-text">
                          在这一部分，我将为您介绍什么是点云配准算法。点云配准算法是一类用于将两个或多个点云数据集对齐或注册的算法，它是计算机视觉、机器人学和计算机图形学中的重要问题，其应用包括三维重建、环境建模、目标识别与跟踪等。在我们的算法设计与应用当中，我们主要设计并实现了以下创新之处：
                    </div>
                </div>

            </div><!-- first row -->
            
            <div class="row tm-content-box"><!-- second row -->
        		<div class="col-lg-1">
                    <i class="far fa-3x fa-chart-bar text-center tm-icon"></i>
                </div>
                <div class="col-lg-5">
                    <div class="tm-intro-text-container">
                        <h2 class="tm-text-primary mb-4">快速变换估计</h2>
                        <p class="mb-4 tm-intro-text">
                          基于YOHO算法提取点云数据局部特征，聚合局部描述子，进而使用NetVlad网络算法构建点云数据的全局特征。基于点云的全局特征估算站与站之间的点云重叠率效率较高，能够实现快速变换估计。</p>
                    </div>
                </div>
                
                <div class="col-lg-1">
                    <i class="far fa-3x fa-comment-alt text-center tm-icon"></i>
                </div>
                <div class="col-lg-5">
                    <div class="tm-intro-text-container">
                        <h2 class="tm-text-primary mb-4">稀疏图构建</h2>
                        <p class="mb-4 tm-intro-text">
                          传统的位姿图构建基于密集图，即两两点云之间均进行配准构造位姿图。本算法设计创新性使用稀疏图构建方案，仅在基于前top-k的重叠度筛选出的配准候选集中进行两两配准，实现高效高利用率。
                        </p>
                    </div>
                </div>

            </div><!-- second row -->
            
            <div class="row tm-content-box"><!-- third row -->
        		<div class="col-lg-1">
                    <i class="fas fa-3x fa-fingerprint text-center tm-icon"></i>
                </div>
                <div class="col-lg-5">
                    <div class="tm-intro-text-container">
                        <h2 class="tm-text-primary mb-4">多站位姿解算</h2>
                        <p class="mb-4 tm-intro-text">
                      基于IRLS（迭代加权最小二乘优化算法）的选权迭代运算，反复更新权重，以逐步逼近最小化加权最小二乘损失函数的目标，从而实现多站点云位姿解算，即所有点云同时在同一全局特征下实现配准，突破了传统的两站点云配准低效耗时的桎梏。</p>
                          
                          <div class="tm-continue">
                            <a href="#testimonials" class="tm-intro-text tm-btn-primary">查看数据集</a>
                        </div>
                    </div>
                </div>
                
                <div class="col-lg-1">
                    <i class="fas fa-3x fa-users text-center tm-icon"></i>
                </div>
                <div class="col-lg-5">
                    <div class="tm-intro-text-container">
                      <h2 class="tm-text-primary mb-4">历史重加权函数</h2>
                        <p class="mb-4 tm-intro-text">
                      由于IRLS早期迭代过程中会出现离群值偏向和无法修剪的问题，设计历史重加权函数，即特定迭代的权重考虑所有先前历史迭代的残差以确定当前迭代的稳健权重，这样就可以实现对离群值的不敏感处理，从而避免局部最优与离群值偏向。 </p>
                          
                          <div class="tm-continue">
                            <a href="#gallery" class="tm-intro-text tm-btn-primary">查看配准效果</a>
                        </div>
                    </div>
                </div>

            </div><!-- third row -->

        </div>
      
    </section>
    
    <section id="testimonials" class="tm-section-pad-top tm-parallax-2">      
      <div class="container tm-testimonials-content">
        <div class="row">
          <div class="col-lg-12 tm-content-box">
            <h2 class="text-white text-center mb-4 tm-section-title">数据集</h2>
            <p class="mx-auto tm-section-desc text-center">
                在这一部分，我们精心挑选了三个在三维重建领域知名的点云数据集，分别是3DMatch、ScanNet以及ETH数据集，以下分别是它们信息的简要介绍。
              </p>
            <div class="mx-auto tm-gallery-container tm-gallery-container-2">
              <div class="tm-testimonials-carousel">
                <figure class="tm-testimonial-item">
                  <img src="img/DxWpZMJC3rSKvey.png" alt="Image" class="img-fluid mx-auto">
                  <blockquote>3DMatch是一个用于室内场景的三维点云配准的数据集和算法。这个数据集包含了来自不同视角和光照条件下的三维点云数据，以及这些点云之间的配准信息。通过这些数据，可以进行室内场景的三维点云配准算法的研究和评估。</blockquote>
                  <figcaption>3DMatch</figcaption>
                </figure>

                <figure class="tm-testimonial-item">
                  <img src="img/2020112809124367.png" alt="Image" class="img-fluid mx-auto">
                  <blockquote>ScanNet是一个用于室内场景的大规模三维重建和语义分割的数据集。这个数据集包含了来自室内环境的RGB图像、深度图像和相机姿态信息。通过这些数据，可以进行室内场景的三维重建、语义分割、物体检测等任务的研究和开发。</blockquote>
                  <figcaption>ScanNet</figcaption>
                </figure>

                <figure class="tm-testimonial-item">
                  <img src="img/34490801.png" alt="Image" class="img-fluid mx-auto">
                  <blockquote>
                    ETH数据集是一组用于计算机视觉和机器人领域的常用数据集，由瑞士苏黎世联邦理工学院（ETH Zurich）提供。这些数据集涵盖了多个子领域，包括室外场景、室内场景、视觉SLAM（同时定位与地图构建）、物体识别、行人检测等。</blockquote>
                  <figcaption>ETH</figcaption>
                </figure>

    
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="tm-bg-overlay"></div>
    </section>
    
    <section id="gallery" class="tm-section-pad-top">
      <div class="container tm-container-gallery">
        <div class="row">
          <div class="text-center col-12">
              <h2 class="tm-text-primary tm-section-title mb-4">效果展示</h2>
              <p class="mx-auto tm-section-desc">
                在这一部分，我们在数据集上应用了我们所设计改良的算法，分别对应着不同数据集中不同场景的点云配准和场景还原，其结果展示如下，您可自行点击查看配准前后效果。
              </p>
          </div>            
        </div>
        <div class="row">
            <div class="col-12">
                <div class="mx-auto tm-gallery-container">
                    <div class="grid tm-gallery">
                      <a href="img/giphy.gif">
                        <figure class="effect-honey tm-gallery-item">
                          <img src="img/giphy.gif" alt="Image 1" class="img-fluid">
                          <figcaption>
                            <h2><i>Physical Health <span>Exercise!</span></i></h2>
                          </figcaption>
                        </figure>
                      </a>
                      <a href="img/gallery-img-02.jpg">
                        <figure class="effect-honey tm-gallery-item">
                          <img src="img/gallery-tn-02.jpg" alt="Image 2" class="img-fluid">
                          <figcaption>
                            <h2><i>Rain on Glass <span>Second Image</span></i></h2>
                          </figcaption>
                        </figure>
                      </a>
                      <a href="img/gallery-img-03.jpg">
                        <figure class="effect-honey tm-gallery-item">
                          <img src="img/gallery-tn-03.jpg" alt="Image 3" class="img-fluid">
                          <figcaption>
                            <h2><i><span>Sea View</span> Mega City</i></h2>
                          </figcaption>
                        </figure>
                      </a>
                      <a href="img/gallery-img-04.jpg">
                        <figure class="effect-honey tm-gallery-item">
                          <img src="img/gallery-tn-04.jpg" alt="Image 4" class="img-fluid">
                          <figcaption>
                            <h2><i>Dream Girl <span>Thoughts</span></i></h2>
                          </figcaption>
                        </figure>
                      </a>
                      <a href="img/gallery-img-05.jpg">
                        <figure class="effect-honey tm-gallery-item">
                          <img src="img/gallery-tn-05.jpg" alt="Image 5" class="img-fluid">
                          <figcaption>
                            <h2><i><span>Workstation</span> Offices</i></h2>
                          </figcaption>
                        </figure>
                      </a>
                      <a href="img/gallery-img-06.jpg">
                        <figure class="effect-honey tm-gallery-item">
                          <img src="img/gallery-tn-06.jpg" alt="Image 6" class="img-fluid">
                          <figcaption>
                            <h2><i>Just Above <span>The City</span></i></h2>
                          </figcaption>
                        </figure>
                      </a>
                      <a href="img/gallery-img-01.jpg">
                        <figure class="effect-honey tm-gallery-item">
                          <img src="img/gallery-tn-01.jpg" alt="Image 7" class="img-fluid">
                          <figcaption>
                            <h2><i>Another <span>Exercise Time</span></i></h2>
                          </figcaption>
                        </figure>
                      </a>
                      <a href="img/gallery-img-02.jpg">
                        <figure class="effect-honey tm-gallery-item">
                          <img src="img/gallery-tn-02.jpg" alt="Image 8" class="img-fluid">
                          <figcaption>
                            <h2><i>Repeated <span>Image Spot</span></i></h2>
                          </figcaption>
                        </figure>
                      </a>
                    </div>
                </div>                
            </div>        
          </div>
      </div>
    </section>

    <!-- Contact -->
    <section id="contact" class="tm-section-pad-top tm-parallax-2">
    
      <div class="container tm-container-contact">
        
        <div class="row">
            
            <div class="text-center col-12">
                <h2 class="tm-section-title mb-4">性能指标</h2>
                <p class="mb-5">
                  在这一部分，由于仅有配准效果的展示并不足以说明我们算法设计与应用的优越性所在，因此我们分别在数据集上对算法性能指标进行了测试，包括但不限于配准召回率、效率、准确率等，其结果展示如下，欢迎您点击浏览。
                </p><br>
            </div>
            
            <div class="col-12">
              <div class="mx-auto tm-gallery-container">
                  <div class="grid tm-gallery">
                    <a href="img/giphy.gif">
                      <figure class="effect-honey tm-gallery-item">
                        <img src="img/giphy.gif" alt="Image 1" class="img-fluid">
                        <figcaption>
                          <h2><i>Physical Health <span>Exercise!</span></i></h2>
                        </figcaption>
                      </figure>
                    </a>
                    <a href="img/gallery-img-02.jpg">
                      <figure class="effect-honey tm-gallery-item">
                        <img src="img/gallery-tn-02.jpg" alt="Image 2" class="img-fluid">
                        <figcaption>
                          <h2><i>Rain on Glass <span>Second Image</span></i></h2>
                        </figcaption>
                      </figure>
                    </a>
                    <a href="img/gallery-img-03.jpg">
                      <figure class="effect-honey tm-gallery-item">
                        <img src="img/gallery-tn-03.jpg" alt="Image 3" class="img-fluid">
                        <figcaption>
                          <h2><i><span>Sea View</span> Mega City</i></h2>
                        </figcaption>
                      </figure>
                    </a>
                    <a href="img/gallery-img-04.jpg">
                      <figure class="effect-honey tm-gallery-item">
                        <img src="img/gallery-tn-04.jpg" alt="Image 4" class="img-fluid">
                        <figcaption>
                          <h2><i>Dream Girl <span>Thoughts</span></i></h2>
                        </figcaption>
                      </figure>
                    </a>
                    <a href="img/gallery-img-05.jpg">
                      <figure class="effect-honey tm-gallery-item">
                        <img src="img/gallery-tn-05.jpg" alt="Image 5" class="img-fluid">
                        <figcaption>
                          <h2><i><span>Workstation</span> Offices</i></h2>
                        </figcaption>
                      </figure>
                    </a>
                    <a href="img/gallery-img-06.jpg">
                      <figure class="effect-honey tm-gallery-item">
                        <img src="img/gallery-tn-06.jpg" alt="Image 6" class="img-fluid">
                        <figcaption>
                          <h2><i>Just Above <span>The City</span></i></h2>
                        </figcaption>
                      </figure>
                    </a>
                    <a href="img/gallery-img-01.jpg">
                      <figure class="effect-honey tm-gallery-item">
                        <img src="img/gallery-tn-01.jpg" alt="Image 7" class="img-fluid">
                        <figcaption>
                          <h2><i>Another <span>Exercise Time</span></i></h2>
                        </figcaption>
                      </figure>
                    </a>
                    <a href="img/gallery-img-02.jpg">
                      <figure class="effect-honey tm-gallery-item">
                        <img src="img/gallery-tn-02.jpg" alt="Image 8" class="img-fluid">
                        <figcaption>
                          <h2><i>Repeated <span>Image Spot</span></i></h2>
                        </figcaption>
                      </figure>
                    </a>
                  </div>
              </div>                
          </div>        
        </div>
            
            
        </div><!-- row ending -->
        
      </div>

      	<footer class="text-center small tm-footer">
          <p class="mb-0">
          Copyright &copy; 2024 中国大学生计算机设计大赛项目-算法设计与应用 
          
          . <a rel="nofollow" href="https://www.tooplate.com" title="HTML templates"></a></p>
        </footer>

    </section>
    
    <script src="js/jquery-1.9.1.min.js"></script>     
    <script src="slick/slick.min.js"></script>
    <script src="magnific-popup/jquery.magnific-popup.min.js"></script>
    <script src="js/easing.min.js"></script>
    <script src="js/jquery.singlePageNav.min.js"></script>     
    <script src="js/bootstrap.min.js"></script> 
    <script>

      function getOffSet(){
        var _offset = 450;
        var windowHeight = window.innerHeight;

        if(windowHeight > 500) {
          _offset = 400;
        } 
        if(windowHeight > 680) {
          _offset = 300
        }
        if(windowHeight > 830) {
          _offset = 210;
        }

        return _offset;
      }

      function setParallaxPosition($doc, multiplier, $object){
        var offset = getOffSet();
        var from_top = $doc.scrollTop(),
          bg_css = 'center ' +(multiplier * from_top - offset) + 'px';
        $object.css({"background-position" : bg_css });
      }

      // Parallax function
      // Adapted based on https://codepen.io/roborich/pen/wpAsm        
      var background_image_parallax = function($object, multiplier, forceSet){
        multiplier = typeof multiplier !== 'undefined' ? multiplier : 0.5;
        multiplier = 1 - multiplier;
        var $doc = $(document);
        // $object.css({"background-attatchment" : "fixed"});

        if(forceSet) {
          setParallaxPosition($doc, multiplier, $object);
        } else {
          $(window).scroll(function(){          
            setParallaxPosition($doc, multiplier, $object);
          });
        }
      };

      var background_image_parallax_2 = function($object, multiplier){
        multiplier = typeof multiplier !== 'undefined' ? multiplier : 0.5;
        multiplier = 1 - multiplier;
        var $doc = $(document);
        $object.css({"background-attachment" : "fixed"});
        
        $(window).scroll(function(){
          if($(window).width() > 768) {
            var firstTop = $object.offset().top,
                pos = $(window).scrollTop(),
                yPos = Math.round((multiplier * (firstTop - pos)) - 186);              

            var bg_css = 'center ' + yPos + 'px';

            $object.css({"background-position" : bg_css });
          } else {
            $object.css({"background-position" : "center" });
          }
        });
      };
      
      $(function(){
        // Hero Section - Background Parallax
        background_image_parallax($(".tm-parallax"), 0.30, false);
        background_image_parallax_2($("#contact"), 0.80);   
        background_image_parallax_2($("#testimonials"), 0.80);   
        
        // Handle window resize
        window.addEventListener('resize', function(){
          background_image_parallax($(".tm-parallax"), 0.30, true);
        }, true);

        // Detect window scroll and update navbar
        $(window).scroll(function(e){          
          if($(document).scrollTop() > 120) {
            $('.tm-navbar').addClass("scroll");
          } else {
            $('.tm-navbar').removeClass("scroll");
          }
        });
        
        // Close mobile menu after click 
        $('#tmNav a').on('click', function(){
          $('.navbar-collapse').removeClass('show'); 
        })

        // Scroll to corresponding section with animation
        $('#tmNav').singlePageNav({
          'easing': 'easeInOutExpo',
          'speed': 600
        });        
        
        // Add smooth scrolling to all links
        // https://www.w3schools.com/howto/howto_css_smooth_scroll.asp
        $("a").on('click', function(event) {
          if (this.hash !== "") {
            event.preventDefault();
            var hash = this.hash;

            $('html, body').animate({
              scrollTop: $(hash).offset().top
            }, 600, 'easeInOutExpo', function(){
              window.location.hash = hash;
            });
          } // End if
        });

        // Pop up
        $('.tm-gallery').magnificPopup({
          delegate: 'a',
          type: 'image',
          gallery: { enabled: true }
        });

        $('.tm-testimonials-carousel').slick({
          dots: true,
          prevArrow: false,
          nextArrow: false,
          infinite: false,
          slidesToShow: 3,
          slidesToScroll: 1,
          responsive: [
            {
              breakpoint: 992,
              settings: {
                slidesToShow: 2
              }
            },
            {
              breakpoint: 768,
              settings: {
                slidesToShow: 2
              }
            }, 
            {
              breakpoint: 480,
              settings: {
                  slidesToShow: 1
              }                 
            }
          ]
        });

        // Gallery
        $('.tm-gallery').slick({
          dots: true,
          infinite: false,
          slidesToShow: 5,
          slidesToScroll: 2,
          responsive: [
          {
            breakpoint: 1199,
            settings: {
              slidesToShow: 4,
              slidesToScroll: 2
            }
          },
          {
            breakpoint: 991,
            settings: {
              slidesToShow: 3,
              slidesToScroll: 2
            }
          },
          {
            breakpoint: 767,
            settings: {
              slidesToShow: 2,
              slidesToScroll: 1
            }
          },
          {
            breakpoint: 480,
            settings: {
              slidesToShow: 1,
              slidesToScroll: 1
            }
          }
        ]
        });
      });
    </script>
  </body>
</html>
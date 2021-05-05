<template>
  <div class="active-dark">
    <!-- Start Header Area -->
    <HeaderOnePageTwo />
    <!-- End Header Area -->
    <!-- Start Slider Area  -->
    <div class="rn-slider-area poss_relative" id="home">
      <div
        class="slide personal-portfolio-slider slider-style-3 slider-paralax bg_image bg_image--25 d-flex align-center"
      >
        <BannerThree>
          <span slot="designation">Visual Designer</span>
          <h1 class="heading-title" slot="heading-title">
            Oh hey there, I am <span>Renata</span> and I am a double belt designer! 
          </h1>
        </BannerThree>
      </div>
    </div>
    <!-- End Slider Area -->

    <!-- Start About Area  -->
    <div class="section about-area rn-section-gap bg_color--1" id="about">
      <div class="about-wrapper">
        <div class="container">
          <AboutFour>
            <img
              slot="thum-img"
              class="w-100"
              src="../../assets/images/about/about-8.jpg"
              alt="About Images"
            />
          </AboutFour>
        </div>
      </div>
    </div>
    <!-- Start About Area  -->

  

    <!-- Start Portfolio Area -->
    <div
      class="section rn-portfolio-area rn-section-gap bg_color--1"
      id="portfolio"
    >
      <v-container>
        <v-row>
          <v-col lg="12">
            <div class="section-title section-title--2 text-center mb--20">
              <h2 class="heading-title">Projects and creative work</h2>
              <p>
                Here you can see some of my newest projects, most of them being academy projects at the moment as I am full time student.
                My projects are usually about visual identity, such as logos and banners. I am working close to several e-sports teams and get to make them needed visuals for places such as twitter.   
              </p>
            </div>
          </v-col>
        </v-row>
        <PortfolioFour />
        <v-row>
          <v-col lg="12">
            
          </v-col>
        </v-row>
      </v-container>
    </div>
    <!-- End Portfolio Area -->

    <!-- Start Blog Area  -->
    <div class="section rn-blog-area rn-section-gap bg_color--5" id="blog">
      <v-container>
        <v-row align="end" class="mb--20">
          <v-col lg="6" md="12">
            <div class="section-title text-left">
              <h2>Hobby art</h2>
              <p>
                I have been passionate artist since I can remember, drawing is one of my favourite pastime activities! Here are some of my newest works! 
                I made digital art that is created using adobe programs, mainly photoshop and illustrator. I use drawing tablet and have knowledge in hardware.  
              </p>
            </div>
          </v-col>
        </v-row>
        <Blog />
      </v-container>
    </div>
    <!-- End Blog Area  -->

    <!-- Start Contact Area  -->
    <div
      class="section rn-contact-area rn-section-gap bg_color--1"
      id="contact"
    >
      <div class="contact-form--1">
        <v-container>
          <Contact>
            <img
              slot="contact-img"
              class="w-100"
              src="../../assets/images/about/about-9.jpg"
              alt="trydo"
            />
          </Contact>
        </v-container>
      </div>
    </div>
    <!-- End Contact Area  -->

    <!-- Start Footer Area  -->
    <Footer />
    <!-- End Footer Area  -->
  </div>
</template>

<script>
  import HeaderOnePageTwo from "../../components/header/HeaderOnePageTwo";
  import BannerThree from "../../components/slider/BannerThree";
  import AboutFour from "../../components/about/AboutFour";
  import ServiceThree from "../../components/service/ServiceThree";
  import PortfolioFour from "../../components/portfolio/PortfolioFour";
  import Blog from "../../components/blog/Blog";


  export default {
    components: {
      HeaderOnePageTwo,
      BannerThree,
      AboutFour,
      ServiceThree,
      PortfolioFour,
      Blog,
    },
    data() {
      return {};
    },
  };
</script>

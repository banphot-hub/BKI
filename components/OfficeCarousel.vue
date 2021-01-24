<template>
  <section class="ofc-caoursel-area area-padding">
      <div class="ofc-caoursel-fluid">
          <div class="container">
              <div class="row">
                  <div class="col-md-12 primary-padding-2 text-center">
                      <div class="avivon-heading">
                          <h2 class="avivon__title six__title">offices near you</h2>
                      </div><!-- end avivon-heading -->
                  </div><!-- end col-md-12 -->
              </div><!-- end row -->
              <div class="row">
                  <div class="col-md-12 no-padding-lr">
                      <div class="office-list">
                        <swiper :options="swiperOptions">
                          <swiper-slide>
                          <div class="office-list-item">
                              <div class="office__name">
                                  <h3 class="office__name-title">Bangkok</h3>
                              </div><!-- end office__name -->
                              <div class="office__desc">
                                  <p class="office__desc-desc">
                                      22 Silom Bangkok
                                      needhelp@open-me.io
                                      888 999 0000</p>
                              </div><!-- end office__desc -->
                          </div><!-- end office-list-item -->
                          </swiper-slide>
                          

                        </swiper>

                        <div class="swiper-pagination owl-dots" slot="pagination"></div>

                      </div><!-- end office-list -->
                  </div><!-- end col-md-12 -->
              </div><!-- end row -->
          </div><!-- container -->
      </div><!-- end ofc-caoursel-fluid -->
  </section>
</template>

<script>
  import { Swiper, SwiperSlide, directive } from 'vue-awesome-swiper';
  import 'swiper/css/swiper.css';
    export default {
      name: "OfficeCarousel",
      components: {
        Swiper,
        SwiperSlide
      },
      directives: {
        swiper: directive
      },
      data() {
        return {
          swiperOptions: {
            slidesPerView : 1,
            loop: true,
            speed: 1000,
            spaceBetween : 30,
            autoplay: {
                delay: 3000,
                disableOnInteraction: false
            },
            pagination: {
              el: '.swiper-pagination',
              type: 'bullets',
              clickable: true
            },
            // Responsive breakpoints
            breakpoints: {
              1024:{
                  slidesPerView : 1
              },
              768:{
                  slidesPerView : 1
              },
              640:{
                  slidesPerView : 1
              },
              320:{
                  slidesPerView : 1
              }
            }
          }
        }
      },

    }
</script>

<style scoped>

</style>

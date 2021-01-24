<template>
  <div>
    <div :class="`body-overlay ${mobileToggle ? 'active' : ''}`"></div>
    <div :class="`offcanvas-menu ${mobileToggle ? 'active' : ''}`">
      <div @click="mobileToggle = !mobileToggle" class="menu__close"></div>
      <!-- end menu__close -->
      <ul class="off__menu">
        <li class="menu__title-only">HOME <i class="fas fa-angle-down"></i></li>
        <li><a href="/">Home</a></li>
        <li class="menu__title-only">
          Services <i class="fas fa-angle-down"></i>
        </li>
        <li><a href="/service1">sประกันบุคลากรแพทย์</a></li>
        <li><a href="/service2">ประกันวินาศภัย</a></li>
        <li><a href="/single-service">ประกันชีวิต</a></li>
        <li class="menu__title-only">
          About <i class="fas fa-angle-down"></i>
        </li>
        <li><a href="/contact">เกี่ยวกับเรา</a></li>
        <li class="menu__title-only">
          Contract <i class="fas fa-angle-down"></i>
        </li>
        <li><a href="/contact">ติดต่อเรา</a></li>
      </ul>
    </div>
    <section :class="`menu-area ${sticky ? 'active' : ''}`">
      <div class="top-menu-area">
        <div class="container-fluid">
          <div class="row">
            <div class="col-md-12">
              <div class="menu-full-width">
                <div :class="`logo-box ${sticky ? 'active' : ''}`">
                  <div @click="mobileToggle = !mobileToggle" class="site-open">
                    <span class="open__only"></span>
                    <span class="open__only"></span>
                    <span class="open__only"></span>
                  </div>
                  <!-- end site-open -->
                  <div class="logo">
                    <nuxt-link to="/" title="Avivon"
                      ><img src="/images/logo.svg" alt="logo"
                    /></nuxt-link>
                  </div>
                  <!-- end logo -->
                </div>
                <!-- end logo-box -->
                <div class="main-menu">
                  <nav class="menu__wrapper">
                    <ul class="dropdown-main">
                      <li>
                        <a href="/">Home</a>
                        <!--     <div class="main__dropdown-menu">
                                                  <ul>
                                                      <li><nuxt-link to="/">home 01</nuxt-link></li>
                                                      <li><nuxt-link to="/index2">home 02</nuxt-link></li>
                                                      <li><nuxt-link to="/index3">home 03</nuxt-link></li>
                                                  </ul>
                                              </div> --><!-- end main__dropdown-menu -->
                      </li>
                      <li>
                        <a href="#">Services</a>
                        <div class="main__dropdown-menu">
                          <ul>
                            <li>
                              <nuxt-link to="/service1"
                                >ประกันบุคลากรแพทย์</nuxt-link
                              >
                            </li>
                            <li>
                              <nuxt-link to="/service2"
                                >ประกันวินาศภัย</nuxt-link
                              >
                            </li>
                            <li>
                              <nuxt-link to="/single-service"
                                >ประกันชีวิต</nuxt-link
                              >
                            </li>
                          </ul>
                        </div>
                        <!-- end main__dropdown-menu -->
                      </li>
                      <!-- <li>
                                              <a href="#">pages</a>
                                              <div class="main__dropdown-menu">
                                                  <ul>
                                                      <li><nuxt-link to="/about-us1">about us 01</nuxt-link></li>
                                                      <li><nuxt-link to="/about-us2">about us 02</nuxt-link></li>
                                                      <li><nuxt-link to="/our-mission">our mission</nuxt-link></li>
                                                      <li><nuxt-link to="/our-history">our history</nuxt-link></li>
                                                      <li><nuxt-link to="/our-partnership">partnership</nuxt-link></li>
                                                  </ul>
                                              </div> 
                                          </li>
                                          <li>
                                              <a href="#">cases</a>
                                              <div class="main__dropdown-menu">
                                                  <ul>
                                                      <li><nuxt-link to="/cases1">cases 01</nuxt-link></li>
                                                      <li><nuxt-link to="/cases2">cases 02</nuxt-link></li>
                                                      <li><nuxt-link to="/single-cases">single case</nuxt-link></li>
                                                  </ul>
                                              </div>
                                          </li>
                                          <li>
                                              <a href="#">blog</a>
                                              <div class="main__dropdown-menu">
                                                  <ul>
                                                      <li><nuxt-link to="/blog-post">blog post</nuxt-link></li>
                                                      <li><nuxt-link to="/single-blog">single blog</nuxt-link></li>
                                                  </ul>
                                              </div> 
                                          </li> -->
                      <li>
                        <nuxt-link to="/about-us1">About Us</nuxt-link>
                      </li>

                      <li>
                        <nuxt-link to="/contact">contact</nuxt-link>
                      </li>
                    </ul>
                  </nav>
                  <!-- end menu__wrapper -->
                  <div class="logo-right-button">
                    <div class="lang-dropdown">
                      <ul>
                        <li>
                          <a href="#">
                            <img src="/images/user.png" alt="English" />
                          </a>
                          <div class="lang-drop-item">
                            <a href="/Login">
                              <img src="/images/login.png" alt="Login" />
                              Login
                            </a>
                            <a href="/Signup">
                              <img src="/images/unlock.png" alt="Login" />
                              Register
                            </a>
                          </div>
                        </li>
                      </ul>
                    </div>
                    <!-- end lang-dropdown -->
                    <div class="contact-para">
                      <p>+ 089 771 1130</p>
                      <span class="fontello icon-phone-call phone-call"></span>
                    </div>
                    <!-- end contact-para -->
                  </div>
                  <!-- end logo-right-button -->
                </div>
                <!-- end main-menu -->
              </div>
              <!-- end menu-full-width -->
            </div>
            <!-- end col-md-12 -->
          </div>
          <!-- end row -->
        </div>
        <!-- end container -->
      </div>
      <!-- end top-menu-area -->
    </section>
  </div>
</template>

<script>
export default {
  name: "NavOne",
  data() {
    return {
      sticky: false,
      mobileToggle: false,
    };
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
  },
  methods: {
    handleScroll() {
      if (window.scrollY > 70) {
        this.sticky = true;
      } else if (window.scrollY < 70) {
        this.sticky = false;
      }
    },
  },
};
</script>

<style scoped></style>

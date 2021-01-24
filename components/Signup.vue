<template>
  <section class="contact-area responsive-content area-padding">
      <div class="contact-fluid">
          <div class="container contact-info avivon-pb">
              <div class="row">
                  <div class="col-md-4 primary-padding">
                      <div class="avivon-heading">
                          <h2 class="avivon__title">Sign Up</h2>
                          <p class="avivon__desc contact__desc mt-50px">
                              เพื่อให้แน่ใจว่าข้อมูลของคุณนั้นปลอดภัย เราให้ความสำคัญและเคารพในความเป็นส่วนบุคคล ลงทะเบียนเพื่อประโยชน์ในการรับข้อมูลจากเรา
                          </p>
                      </div><!-- end avivon-heading -->
                  </div><!-- end col-md-4 -->
                  <div class="col-md-8">
                      <div class="comment__form contact__form">
                          <form action="#">
                              <div class="input__box-input">
                                  <input type="text" placeholder="Your name">
                              </div>
                              <div class="input__box-input email-box">
                                  <input type="email" placeholder="Your email">
                              </div>
                               <div class="input__box-input email-box">
                                  <input type="password" placeholder="Password">
                              </div>
                              <div class="input__box-input email-box">
                                  <input type="password" placeholder="Confirm password">
                              </div>
                              <!-- <textarea name="message" placeholder="message"></textarea> -->
                              <button class="submit__btn-btn">Register
                                  <span class="fontello icon-angle-double-right"></span>
                              </button>
                              <nuxt-link to="/">
                              <button class="submit__btn-btn">Cancel
                                  <span class="fontello icon-angle-double-right"></span>
                              </button>
                              </nuxt-link>
                          </form>
                      </div><!-- end comment__form -->
                  </div><!-- end col-md-8 -->
              </div><!-- end row -->
          </div><!-- container -->
      </div><!-- end contact-fluid -->
  </section>
</template>

<script>
    export default {
        name: "Signup"
    }
</script>

<style scoped>

</style>

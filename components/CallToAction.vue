<template>
  <section class="clta-area area-padding-2 theme-bg-gray">
      <div class="clta-bg"></div>
      <div class="clta-fluid">
          <div class="container">
              <div class="row">
                  <div class="col-md-3">
                      <div class="avivon-heading white-heading">
                          <h2 class="avivon__title">let’s make a call request now.</h2>
                      </div><!-- end avivon-heading -->
                  </div><!-- end col-md-3 -->
                  <div class="col-md-9 shared-form-box">
                      <div class="col-md-6">
                          <div class="shared-form">
                              <form action="#">
                                  <input type="text" placeholder="business planing">
                                  <input type="text" placeholder="your name">
                                  <input class="input__number" type="text" placeholder="phone number">
                              </form>
                          </div><!-- end shared-form -->
                      </div><!-- end col-md-6 -->
                      <div class="col-md-6">
                          <div class="shared-form">
                              <textarea name="message" placeholder="message"></textarea>
                              <button class="form__btn" value="submit">
                                  get started <span class="fontello icon-angle-double-right"></span>
                              </button>
                          </div><!-- end shared-form -->
                      </div><!-- end col-md-6 -->
                  </div><!-- end col-md-9 -->
              </div><!-- end row -->
          </div><!-- container -->
      </div><!-- end clta-fluid -->
  </section>
</template>

<script>
    export default {
        name: "CallToAction"
    }
</script>

<style scoped>

</style>

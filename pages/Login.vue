<template>
  <div>
    <NavOne />
    <LoginPageHeder title="Login" />
    <Login />
    <Footer />
  </div>
</template>
<script>
  import NavOne from "../components/NavOne";
  import LoginPageHeder from "../components/LoginPageHeader";
  import Footer from "../components/Footer";
 
  import Login from "../components/Login";
  export default {
    components: {Login, Footer, LoginPageHeder, NavOne}
  }
</script>
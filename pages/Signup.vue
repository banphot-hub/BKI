<template>
  <div>
    <NavOne />
    <PageHeader title="contact us" />
    <Signup />
    <OfficeCarousel />
    <MapG />
    <Footer />
  </div>
</template>
<script>
  import NavOne from "../components/NavOne";
  import PageHeader from "../components/PageHeader";
  import Footer from "../components/Footer";
  import OfficeCarousel from "../components/OfficeCarousel";
  import MapG from "../components/MapG";
  import Signup from "../components/Signup";
  export default {
    components: {Signup, MapG, OfficeCarousel, Footer, PageHeader, NavOne}
  }
</script>
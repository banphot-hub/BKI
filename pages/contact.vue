<template>
  <div>
    <NavOne />
    <ContactPageHeader title="contact us" />
    <Contact />
    <OfficeCarousel />
    <MapG />
    <Footer />
  </div>
</template>
<script>
  import NavOne from "../components/NavOne";
  import ContactPageHeader from "../components/ContractPageHeader";
  import Footer from "../components/Footer";
  import OfficeCarousel from "../components/OfficeCarousel";
  import MapG from "../components/MapG";
  import Contact from "../components/Contact";
  export default {
    components: {Contact, MapG, OfficeCarousel, Footer, ContactPageHeader, NavOne}
  }
</script>

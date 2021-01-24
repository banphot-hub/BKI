<template>
  <div>
    <NavOne />
    <AboutPageHeader title="about Us" />
    <ThinkAreaThree />
    <!-- <FunFact /> -->
    <!-- <Team /> -->
    <!-- <TestimonialTwo /> -->
    <!-- <OfferThree /> -->
    <!-- <ClientsLogo /> -->
    <!-- <Meet /> -->
    <Footer />
  </div>
</template>
<script>
  import NavOne from "../components/NavOne";
  import AboutPageHeader from "../components/AboutUsPage";
  import Footer from "../components/Footer";
  import ThinkAreaThree from "../components/ThinkAreaThree";
  import FunFact from "../components/FunFact";
  import Team from "../components/Team";
  import TestimonialTwo from "../components/TestimonialTwo";
  import OfferThree from "../components/OfferThree";
  import ClientsLogo from "../components/ClientsLogo";
  import Meet from "../components/Meet";
  export default {
    components: {
      Meet,
      ClientsLogo,
      OfferThree,
      TestimonialTwo,
      Team,
      FunFact,
      ThinkAreaThree,
      Footer,
      AboutPageHeader,
      NavOne
    },
    head(){
      return {
        title: "Avivon | About"
      }
    }

  }
</script>


/* --------------------------------- script --------------------------------- */
<script>

  import MainServicesSection from './AppMainComponents/MainServicesSection.vue';
  import MainAboutUsSection from './AppMainComponents/MainAboutUsSection.vue';
  import MainProjectSection from './AppMainComponents/MainProjectSection.vue';
  import MainTestimonialSection from './AppMainComponents/MainTestimonialSection.vue';

  export default{
    data(){
      return{



      }
    },
    components:{
      MainServicesSection,
      MainAboutUsSection,
      MainProjectSection,
      MainTestimonialSection,
    }
  }

</script>


/* -------------------------------- template -------------------------------- */
<template>

  <div>
    <MainServicesSection></MainServicesSection>
    <MainAboutUsSection></MainAboutUsSection>
    <MainProjectSection></MainProjectSection>
    <MainTestimonialSection></MainTestimonialSection>

  </div>

</template>


/* ---------------------------------- style --------------------------------- */
<style lang="scss" scoped>



</style>

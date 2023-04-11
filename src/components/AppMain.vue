
/* --------------------------------- script --------------------------------- */
<script>

  import MainServicesSection from './AppMainComponents/MainServicesSection.vue';
  import MainAboutUsSection from './AppMainComponents/MainAboutUsSection.vue';
  import MainProjectSection from './AppMainComponents/MainProjectSection.vue';
  import MainTestimonialSection from './AppMainComponents/MainTestimonialSection.vue';
  import MainBlogSection from './AppMainComponents/MainBlogSection.vue';
  import MainLetsTalkSection from './AppMainComponents/MainLetsTalkSection.vue';

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
      MainBlogSection,
      MainLetsTalkSection,
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
    <MainBlogSection></MainBlogSection>
    <MainLetsTalkSection></MainLetsTalkSection>

  </div>

</template>


/* ---------------------------------- style --------------------------------- */
<style lang="scss" scoped>



</style>

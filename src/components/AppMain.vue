
/* --------------------------------- script --------------------------------- */
<script>

  import MainServicesSection from './AppMainComponents/MainServicesSection.vue';
  import MainAboutUsSection from './AppMainComponents/MainAboutUsSection.vue';

  export default{
    data(){
      return{



      }
    },
    components:{
      MainServicesSection,
      MainAboutUsSection,
    }
  }

</script>


/* -------------------------------- template -------------------------------- */
<template>

  <div>
    <MainServicesSection></MainServicesSection>
    <MainAboutUsSection></MainAboutUsSection>

  </div>

</template>


/* ---------------------------------- style --------------------------------- */
<style lang="scss" scoped>



</style>

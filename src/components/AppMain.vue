
/* --------------------------------- script --------------------------------- */
<script>

  import MainServicesSection from './AppMainComponents/MainServicesSection.vue';
  import MainAboutUsSection from './AppMainComponents/MainAboutUsSection.vue';
  import MainProjectSection from './AppMainComponents/MainProjectSection.vue';

  export default{
    data(){
      return{



      }
    },
    components:{
      MainServicesSection,
      MainAboutUsSection,
      MainProjectSection,
    }
  }

</script>


/* -------------------------------- template -------------------------------- */
<template>

  <div>
    <MainServicesSection></MainServicesSection>
    <MainAboutUsSection></MainAboutUsSection>
    <MainProjectSection></MainProjectSection>

  </div>

</template>


/* ---------------------------------- style --------------------------------- */
<style lang="scss" scoped>



</style>

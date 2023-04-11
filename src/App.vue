
/* --------------------------------- script --------------------------------- */
<script>
  import AppHeader from "./components/AppHeader.vue";
  import AppMain from "./components/AppMain.vue";
  import AppFooter from "./components/AppFooter.vue";

  export default{

    data(){
      return{



      }
      
    },

    components:{
      AppHeader,
      AppMain,
      AppFooter,

    },

    methods:{
      scrollToTop(){
        window.scrollTo({
          top:0,
        })
      }
    },

    
  }

</script>


/* -------------------------------- template -------------------------------- */
<template>

  <div id="page">

    <AppHeader></AppHeader>
    <AppMain></AppMain>
    <AppFooter></AppFooter>

    <div id="fixed-items">
      <div id="top" @click="scrollToTop()"><i class="fa-solid fa-arrow-up"></i></div>
      <div id="message"><i class="fa-regular fa-comment"></i></div>
    </div>

  </div>

</template>


/* ---------------------------------- style --------------------------------- */
<style lang="scss" scoped>

#page{
  position: relative;
}
#fixed-items{
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;

  position: fixed;
  bottom: 20px;
  right: 20px;

  #top{
    display: flex;
    justify-content: center;
    align-items: center;
    
    width: 30px;
    height: 30px;
    
    background-color: white;
    color: black;
    border: 1px solid black;
    padding: 10px;
    border-radius: 50%;
  }
  
  #message{
    display: flex;
    justify-content: center;
    align-items: center;
    
    width: 60px;
    height: 60px;
    
    background-color: #517ceb;
    color: white;
    font-size: 1.6em;
    padding: 10px;
    border-radius: 50%;
  }
}
  
</style>

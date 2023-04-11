
/* --------------------------------- script --------------------------------- */
<script>
  import AppNavbar from './AppNavbar.vue';

  export default{
    data(){
      return{



      }
    },
    components:{
      AppNavbar,
    }
  }

</script>


/* -------------------------------- template -------------------------------- */
<template>

  <header>

    <AppNavbar></AppNavbar>

    <div id="header-inner" class="centered">

      <!-- header texts -->
      <span class="section-title">Always the best way you need it</span>
      <h1>The Best <br> Business <br> Consulting</h1>

      <!-- header buttons -->
      <div id="buttons">
        <button class="btn btn-primary">Read More</button>
        <button id="play-btn"><i class="fa-solid fa-play"></i></button>
      </div>

    </div>

  </header>

</template>


/* ---------------------------------- style --------------------------------- */
<style lang="scss" scoped>

header{
  background-color: #1e1e38;
  background-image: url('../../public/img/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg');
  background-position: right top;
  background-repeat: no-repeat;
  background-size: 60%;

  #header-inner{
    display: flex;
    flex-direction: column;
    gap: 20px;

    padding: 200px 0;

    h1{
      text-transform: uppercase;
      font-weight: bold;
      font-size: 5em;
      
      line-height: 100%;
    }
  }

  #buttons{
    display: flex;
    justify-content: start;
    align-items: end;
    gap: 30px;

    padding: 20px 0;

    #play-btn{
      width: 40px;
      height: 40px;

      padding: 10px;

      color: #39ffbf;
      background-color: transparent;
      border: 1px solid white;
      border-radius: 50%;

      &:hover{
        color: #f81d39;
      }

    }
  }

}

</style>

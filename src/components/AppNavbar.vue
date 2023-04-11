
/* --------------------------------- script --------------------------------- */
<script>

  export default{
    data(){
      return{

        navbarLinks:[
          "Home",
          "About",
          "Projects",
          "Services",
          "Blog",
          "Contact",
        ],

        activeLink: 0,


      }
    },

    methods:{
      changeActiveLink(index){
        this.activeLink = index;
      }
    }
  }

</script>


/* -------------------------------- template -------------------------------- */
<template>

  <nav class="centered">

    <div id="navbar-logo">
      <img src="../../public/img/logotype.png" alt="logo">
    </div>

    <ul id="links">
      <li v-for="(link, index) in navbarLinks" @click="changeActiveLink(index)" >
        <a href="#" :class="index == this.activeLink ? 'active' : '' ">{{ link }}</a>
      </li>
    </ul>

  </nav>

</template>


/* ---------------------------------- style --------------------------------- */
<style lang="scss" scoped>

  nav{
    display: flex;
    justify-content: space-between;
    align-items: center;

  }

  #navbar-logo{
    width: 100px;

    img{
      width: 100%;
    }
  }

  // ul links
  #links{
    display: flex;

    // single link
    li{

      padding: 20px;
      text-transform: uppercase;

      position: relative;
  
      // active link
      a{

        color: rgba(255, 255, 255, 0.7);
        font-size: .8em;
        
        &.active{
          
          text-shadow: 1px 0 white;
          color: white;
          
          &::before{
            content: '';
            position: absolute;
            top: 0;
            left: 50%;
            transform: translate(-50%);
            width: 50px;
            height: 2px;
            background-color: white;
            
            
          }
          
        }
        
      }
    }
  }



</style>

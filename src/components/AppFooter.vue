
/* --------------------------------- script --------------------------------- */
<script>

  import {store} from './../store.js';

  export default{
    data(){
      return{

        store,

      }
    }
  }

</script>


/* -------------------------------- template -------------------------------- */
<template>

  <footer>

    <div id="footer-inner" class="centered">

      <!-- footer top -->
      <div id="footer-top">

        <div id="logo">
          <img src="../../public/img/logotype-2-139x23.png" alt="">
        </div>


        <ul id="links">
          <li v-for="link in store.links">
            <a href="#">{{ link }}</a>
          </li>
        </ul>

        <div id="socials">
          <a href="#">
            <i class="fa-brands fa-instagram"></i>
          </a>

          <a href="#">
            <i class="fa-brands fa-linkedin-in"></i>
          </a>

          <a href="#">
            <i class="fa-brands fa-facebook-f"></i>
          </a>

          <a href="#">
            <i class="fa-brands fa-twitter"></i>
          </a>

        </div>

      </div>

      <!-- footer bottom -->
      <div id="footer-bottom">

        <div id="privacy">
          <span>Terms of use</span>
          <span>Privecy Environtmental Policy</span>
        </div>

        <div id="copyright">
          <span>Copyright © 2020 Phlox Consulting. All Rights Reserved.</span>
        </div>
      </div>

    </div>

  </footer>

</template>


/* ---------------------------------- style --------------------------------- */
<style lang="scss" scoped>

footer{
  background-color: #1e1e38;

  
  #footer-top{
    display: flex;
    justify-content: space-between;
    
    padding: 80px 0;
    border-bottom: .5px solid #626172;

    #logo{
      width: 120px;

      img{
        width: 100%;
      }
    }

    #links{
      display: flex;
      gap: 20px;

      a{
        text-transform: uppercase;
        color: #626172;
        font-size: .9em;

        &:hover{
          text-decoration: underline;
        }
      }
    }

    #socials{
      display: flex;

      color: white;

      a{
        padding: 0 10px;

        &:hover{
          color:#f81d39;
        }
      }

    }
  }

  #footer-bottom{
    display: flex;
    justify-content: space-between;

    color: #626172;
    font-size: .8em;

    padding: 30px 0;

    #privacy{
      display: flex;
      flex-direction: column;
    }
  }
}

</style>

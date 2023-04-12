
/* --------------------------------- script --------------------------------- */
<script>

  export default{
    data(){
      return{



      }
    }
  }

</script>


/* -------------------------------- template -------------------------------- */
<template>

  <section id="about-us">

    <div id="about-us-top">
      
      <!-- left img -->
      <div id="img-container">
        <img src="../../../public/img/business-people-working-together-on-project-and-5FHSKBL.jpg" alt="">
      </div>
      
      <!-- right texts -->
      <div id="texts">
        <span class="section-title">about us</span>
        <h2>we make your strategy work</h2>
        <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed when I hear the buzz of the little world among the stalks,and grow familiar indescribable forms of the insects and flies, then I feel the presence of the Almighty.</p>
      </div>

    </div>
    
    <!-- bottom section -->
    <div id="about-us-bottom" >
      <div id="background-fill"></div>
      <div id="about-us-bottom-inner" class="centered">

        <span id="subtitle">we help to deliver the business case</span>
        <span id="paragraph">When, while lovely valley teems with vapour around meand meridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown</span>
        
        <div id="start-button">
          <button class="btn btn-red">
            Get Started
            <div id="button-background"></div>
          </button>
        </div>
      </div>
    </div>

  </section>

</template>


/* ---------------------------------- style --------------------------------- */
<style lang="scss" scoped>

  #about-us{
    display: flex;
    flex-direction: column;

    background-color: #1e1e38;

    #about-us-top{
      display: flex;

      #img-container{
        width: 50%;
        
        img{
          display: block;
          width: 100%;
        }
      }
      
      #texts{
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 30px;
        
        padding: 0 50px;
        
        width: 50%;
        
        h2{
          font-size: 3em;
          text-transform: uppercase;
          line-height: 100%;
          max-width: 600px;
          
        }
        
        p{
          color: #aaaaaa;
          max-width: 600px;
        }
      }
    }
      
    #about-us-bottom{
      width: 100%;

      position: relative;

      #background-fill{
        position: absolute;
        top: 0;
        left: 0;

        height: 100%;
        width: calc(100% - 1200px);

        background-color: #35ffbf;
        

      }
      
      #about-us-bottom-inner{
        display: flex;
        justify-content: space-around;
        background-color: #35ffbf;
        width: 100%;
  
        padding: 80px;
  
        position: relative;

        #subtitle{
          color: black;
          font-size: 1.4em;
          font-weight: bold;
          text-transform: uppercase;
          
          max-width: 400px;
          
        }
        
        #paragraph{
          max-width: 400px;
          color: #444444;
        }
        
        #start-button{
          position: absolute;
          bottom: 0;
          right: 0;
          
        }

      }
    }
  }

</style>

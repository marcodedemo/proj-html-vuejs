
/* --------------------------------- script --------------------------------- */
<script>

  export default{
    data(){
      return{

        images:[
          "DRY-1-790x592.jpg",
          "221bf0b7-8134-43bb-936a-5acbe42db64a-790x592.jpg",
          "z1el4c4p-790x592.jpg"
        ]

      }
    }
  }

</script>


/* -------------------------------- template -------------------------------- */
<template>

  <section id="project-section">

    <div id="project-inner" class="centered">

      <div id="texts">
        <span class="section-title">Project</span>
        <h2>Our Expert Trusted Consultants Help Clients</h2>

        <div id="slide-buttons">
          <button><i class="fa-solid fa-arrow-left"></i></button>
          <button><i class="fa-solid fa-arrow-right"></i></button>
        </div>

      </div>
      
      <div id="images">

        <div v-for="image in images" id="image">

          <img  :src="'../../../public/img/' + image " alt="">

          <div id="product-info">
            <span id="title">Purinky Products</span>
            <span id="category">uncategorized</span>
          </div>

          <div id="add">
            <i class="fa-solid fa-plus"></i>
          </div>

        </div>

      </div>
      
    </div>
  </section>

</template>


/* ---------------------------------- style --------------------------------- */
<style lang="scss" scoped>

#project-section{
  background-color: #1e1e38;

  #project-inner{
    display: flex;
    flex-direction: column;
    gap: 30px;

    padding: 80px 0 ;


    #texts{
      display: flex;
      flex-direction: column;
      gap: 10px;

      position: relative;

      h2{
        font-size: 2em;
        text-transform: uppercase;
        max-width: 700px;
      }

      #slide-buttons{
        display: flex;
        gap: 5px; 

        position: absolute;
        right: 0;
        top: 50%;
        transform: translateY(-50%);

        button{
          border: none;
          background-color: #36354b;
          padding: 14px;
        }
      }
    }
    
    #images{
      display: flex;
      gap: 30px;

      #image{

        width: calc(100% / 3 );

        position: relative;

        overflow: hidden;

        img{
          width: 100%;
          height: 100%;

          transition: transform 1.2s ease;

        }

        &::after{
          content: '';
  
          display: block;

          position: absolute;
          top: 0;
          right: 0;
  
          width: 100%;
          height: 100%;
          background-color: red;
          mix-blend-mode: darken;
          opacity: 0;
          
          transition: opacity 1.2s;

        }

        &:hover::after{
          opacity: 1;
        }

        &:hover img{
          transform: scale(1.5);
        }

        &:hover #add{
          transform: translateY(-20px);
        }
        &:hover #product-info{
          transform: translateY(-20px);
        } 
        
        #product-info{
          display: flex;
          flex-direction: column;

          position: absolute;
          bottom: 0;
          left: 20px;

          transform: translateY(100px);

          color: white;
          z-index: 2;

          transition: transform 1.2s ease;

          #title{
            font-weight: bold;
          }

          #category{
            color: #ffffff8d;
          }
        }


        #add{
          display: flex;
          justify-content: center;
          align-items: center;

          position: absolute;
          bottom: 0;
          right: 20px;

          transform: translateY(100px);

          width: 50px;
          height: 50px;

          background-color: #1e1e38;
          

          z-index: 2;

          transition: transform 1.2s ease;


        }
      }

    }
  }
}
  
</style>

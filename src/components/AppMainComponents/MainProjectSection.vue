
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
        <img v-for="image in images" :src="'../../../public/img/' + image " alt="">
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
      
      img{
        width: calc(100% / 3 );
      }
    }
  }
}
  
</style>


/* --------------------------------- script --------------------------------- */
<script>

  export default{
    data(){
      return{

        customerOpinions:[
          {
            name:"Vera Duncan",
            company:"Amazon Inc.",
            comment:"When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little.",
            img:"oliver-ragfelt-488196-2.jpg",

          },
          {
            name:"Vera Duncan",
            company:"Amazon Inc.",
            comment:"When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little.",
            img:"oliver-ragfelt-488196-unsplash.jpg",
          
          },
          {
            name:"Vera Duncan",
            company:"Amazon Inc.",
            comment:"When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little.",
            img:"12679.jpg"
          
          },
        ]


      }
    }
  }

</script>


/* -------------------------------- template -------------------------------- */
<template>

  <section id="testimonial">

    <!-- testimonial top section -->
    <div id="testimonial-top" class="centered">

      <!-- texts -->
      <div id="texts">
        <span id="main-section-title">Testimonial</span>
        <h2>What's the customer say about our work</h2>
      </div>
      
    </div>

    <!-- testimonial bottom section -->
    <div id="testimonial-bottom">

      <!-- opinions -->
      <div id="customer-opinions">

        <div v-for="customerOpinion in customerOpinions" class="opinion">

          <div id="hover-background">
            <img :src="'../../../public/img/' + customerOpinion.img" alt="">
          </div>

          <p class="comment">{{ customerOpinion.comment }}</p>
          <span class="name">{{ customerOpinion.name }}</span>
          <span class="company">{{ customerOpinion.company }}</span>
        </div>

      </div>

    </div>

  </section>

</template>


/* ---------------------------------- style --------------------------------- */
<style lang="scss" scoped>

#testimonial{
  background-color: #1e1e38;
  padding-top: 80px;

  #testimonial-top{

    padding-bottom: 50px;

    #texts{
      display: flex;
      flex-direction: column;
      position: relative;


      #main-section-title{
        align-self: center;
        text-transform: uppercase;

        &::before{
        content: '';
        position: absolute;

        top: 16px;
        right: 0;

        height: 2px;
        width: 30px;
        background-color:#39ffbf ;
        }
      }

      h2{
        align-self: end;
        font-size: 2em;
        text-transform: uppercase;
        max-width: 500px;
        text-align: end;
      }
    }
  }

  #testimonial-bottom{
    display: flex;
    justify-content: end;

    #customer-opinions{
      display: flex;
      
      background-color: white;
      color: #aaaaaa;

      width: 90%;

      
      .opinion{
        display: flex;
        flex-direction: column;

        width: calc(100% / 3);

        padding: 80px;

        position: relative;

        overflow-y: hidden;
        
        &:hover #hover-background{
          display: block;
        }

        #hover-background{
          display: none;

          width: 100%;

          position: absolute;
          top: 50%;
          right: 0;

          transform: translateY(-50%);



          img{
            width: 100%;
          }
        }

        .comment{
          max-width: 350px;
          padding-bottom: 30px;
          z-index: 2;
        }

        .name{
          font-weight: bold;
          color: #1e1e38;
          font-size: 1.2em;
          z-index: 2;
        }

        .company{
          font-size: .8em;
          z-index: 2;
        }
      }

    }
  }
}

</style>

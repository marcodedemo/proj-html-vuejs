
/* --------------------------------- script --------------------------------- */
<script>

  export default{
    data(){
      return{

        services:[
          {
            title:"statistical consulting",
            description:"When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a",
            icon:"fa-solid fa-chart-line"
            
          },
          {
            title:"digital consulting",
            description:"When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a",
            icon:"fa-solid fa-bullhorn",

            
          },
          {
            title:"banking consulting",
            description:"When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a",
            icon:"fa-solid fa-wallet",
            
          },
          {
            title:"enterprise consulting",
            description:"When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a",
            icon:"fa-solid fa-bullseye",
            
          },
        ]

      }
    }
  }

</script>


/* -------------------------------- template -------------------------------- */
<template>

  <section id="services" >

    <div id="services-inner" class="centered">

      <h3>Our Consultants Can Help You</h3>
      
      <!-- services list -->
      <div id="services-list">

        <div class="service" v-for="service in services ">
          <!-- icon -->
          <div class="icon"><i :class="service.icon"></i></div>

          <!-- texts -->
          <div id="service-texts">

            <h4 class="title">{{ service.title }}</h4>
            <span class="description">{{ service.description }}</span>

          </div>

        </div>

      </div>

    </div>

  </section>

</template>


/* ---------------------------------- style --------------------------------- */
<style lang="scss" scoped>
  #services{

    padding: 100px 0;

    background-color: white;
    color: black;

    overflow-x: hidden;

    #services-inner{

      padding: 0 100px;
      
      h3{
        text-transform: uppercase;
        color: #1e1e38;
        font-size: 1.5em;
        
        position: relative;
        
        &::after{
          content: '';
          position: absolute;
          
          top: 50%;
          left: auto;
          
          height: 2px;
          width: 100vw;
          margin: 0 30px;
          
          background-color:#39ffbf ;
        }
      }

      #services-list{
        display: flex;
        flex-wrap: wrap;
        gap: 80px;

        margin-top: 80px;
        
        .service{
          
          display: flex;
          gap: 30px;
          
          width: calc(100% / 2 - 80px / 2);
          
          .icon{

            display: flex;
            justify-content: center;
            align-items: center;

            font-size: 1.8em;

            height: 50px;
            width: 50px;

            color: white;
            background-color: #f81d39;
            border-radius: 50%;

            padding: 10px 12px;

          }

          #service-texts{
            display: flex;
            flex-direction: column;
            gap: 15px;
            .title{
              text-transform: uppercase;
              font-size: 1.2em;
            }
          }

        }
      }
    }
    
  }

</style>

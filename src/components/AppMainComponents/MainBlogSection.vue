
/* --------------------------------- script --------------------------------- */
<script>

  export default{
    data(){
      return{

        news:[
          {
            img:"startup-business-people-and-strategy-board-PAJ3P9K-1390x1042.jpg",
            date:"july 4, 2019",
            writer:"paul",
            title:"Canadian Consulting Firm acquired by UK Giant",
            text:"When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a ...",

          },
          {
            img:"business-people-working-together-on-project-and-5FHSKBL-1390.jpg",
            date:"july 4, 2019",
            writer:"paul",
            title:"Canadian Consulting Firm acquired by UK Giant",
            text:"When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a ...",
          }
        ]

      }
    }
  }

</script>


/* -------------------------------- template -------------------------------- */
<template>

  <section id="blog-section">

    <div id="blog-inner" class="centered">

      <!-- texts - title - button -->
      <div id="texts">
        <span class="section-title">Blog</span>
        <h2>The recent news you must read it</h2>

        <button class="btn btn-green">
          View All
          <div id="button-background"></div>
        </button>

      </div>
      
      <!-- news image + info -->
      <div id="news">
        <div v-for="news in news" class="single-news">
          <img :src="'../../../public/img/' + news.img" alt="">

          <!-- news div info -->
          <div class="news-info">
            <span id="date">{{ news.date }}</span>
            <span id="writer"> by {{ news.writer }}</span>
            <div id="title">{{ news.title }}</div>
            <p id="text">{{ news.text }}</p>
          </div>
        </div>
      </div>

    </div>

  </section>

</template>


/* ---------------------------------- style --------------------------------- */
<style lang="scss" scoped>

#blog-section{
  background-color: #1e1e38;

  padding: 200px 0;

  #texts{
    position: relative;


    h2{
      font-size: 2em;
      text-transform: uppercase;
    }

    button{
      position: absolute;
      bottom: 0;
      right: 0;
    }
  }

  #news{
    display: flex;
    gap: 30px;

    padding-top: 50px;

    .single-news{
      width: calc(100% / 2 - 30px / 2);

      position: relative;

      img{
        width: 100%;
      }

      .news-info{
        position: absolute;
        right: 0;
        bottom: -100px;

        width: 400px;

        background-color: white;
        padding: 30px 50px;

        #date{
          color: red;
          
        }

        #writer{
          color: red;
          padding-left: 30px;
        }

        #title{
          color: black;
          font-weight: bold;
          font-size: 1.4em;
          line-height: 100%;
          padding-top: 20px;
        }

        #text{
          color: #aaaaaa;
          padding-top: 20px ;
        }
      }
    }
  }
}

</style>

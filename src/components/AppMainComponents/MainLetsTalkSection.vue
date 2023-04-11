
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

  <section id="lets-talk">

    <div id="content">
        <h2>Let's Talk About Work</h2>
        <span>A wonderful serenity has taken possession Far far away, behind the word mountains.</span>
        <button class="btn black-btn">Get Started</button>
    </div>

  </section>

</template>


/* ---------------------------------- style --------------------------------- */
<style lang="scss" scoped>

#lets-talk{
    background-image: url("../../../public/img/business-people-working-together-on-project-and-B3MZ4TX.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    padding: 200px 0;

    #content{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
        gap: 10px;

        h2{
            font-size: 2em;
            text-transform: uppercase;
        }

        span{
            max-width: 400px;
        }

        .black-btn{
            background-color:#1e1e38 ;
            color: white;
        }
    }
}

</style>

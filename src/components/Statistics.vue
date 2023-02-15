<script>
export default {
name: 'Jumbo',

  data () {
      return{

      }
  },

  components:{},
  methods:{},

}
</script>

<template>

    <div class="statistics-big-container">

        <svg class="svg-uno" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#fff" fill-opacity="1" d="M0,256L120,229.3C240,203,480,149,720,144C960,139,1200,181,1320,202.7L1440,224L1440,320L1320,320C1200,320,960,320,720,320C480,320,240,320,120,320L0,320Z"></path></svg>


        <div class="statistics-small-container d-flex justify-content-between">
        
            <div class="statistic">
                <font-awesome-icon icon="fa-solid fa-suitcase" class="icon"/>                
                <h4>3534</h4>
                <p>planning aplications</p>
            </div>

            <div class="statistic">
                <font-awesome-icon icon="fa-solid fa-building" class="icon"/>
                <h4>896</h4>
                <p>completed projects</p>
            </div>

            <div class="statistic">
                <font-awesome-icon icon="fa-solid fa-users" class="icon"/>
                <h4>172</h4>
                <p>trained professionals</p>
            </div>

            <div class="statistic">
                <font-awesome-icon icon="fa-solid fa-globe" class="icon"/>
                <h4>19</h4>
                <p>international offices</p>
            </div>

        </div>

        <svg class="svg-due" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#fff" fill-opacity="1" d="M0,256L120,229.3C240,203,480,149,720,144C960,139,1200,181,1320,202.7L1440,224L1440,320L1320,320C1200,320,960,320,720,320C480,320,240,320,120,320L0,320Z"></path></svg>    
    
    </div>

</template>

<style lang="scss">

.statistics-big-container{
    background-image: url(../img/home-244125289.jpg);
    padding: 300px;
    background-size: cover;
    position: relative;

    .statistics-small-container{

        .statistic{
            text-align: center;
            color: $main-yellow;

            .icon{
                font-size: 3rem;
                margin-bottom: 15px;
            }

            h4{
                font-weight: 700;
            }
            
            p{
                color: white;
                text-transform: uppercase;
                font-size: 0.8rem;
            }
        }
    }

    .svg-uno{
        position: absolute;
        left: 0;
        top: -50px;
        transform: rotate(180deg);
    }
    .svg-due{
        position: absolute;
        left: 0;
        bottom: -50px;
    }
}

</style>
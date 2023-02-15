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

    <div class="reviews-big-container">

        <svg class="svg-uno" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#f5f5f5" fill-opacity="1" d="M0,256L120,229.3C240,203,480,149,720,144C960,139,1200,181,1320,202.7L1440,224L1440,320L1320,320C1200,320,960,320,720,320C480,320,240,320,120,320L0,320Z"></path></svg>


        <div class="review-small-container">
        
            <h3>Our Home Owners Say</h3>

            <hr>

            <div class="account-img">
            </div>

            <i>
                <p>“No man but feels more of a man in the world if he have but a bit of ground that he can call his own. However small it is on the surface, it is four thousand miles deep; and that is a very handsome property.”</p>
            </i>

            <strong>
                <p>HARRY SMITH - NEW HOME OWNER</p>
            </strong>

        </div>

        <svg class="svg-due" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#f5f5f5" fill-opacity="1" d="M0,256L120,229.3C240,203,480,149,720,144C960,139,1200,181,1320,202.7L1440,224L1440,320L1320,320C1200,320,960,320,720,320C480,320,240,320,120,320L0,320Z"></path></svg>    
    
    </div>

</template>

<style lang="scss">

.reviews-big-container{
    background-image: url(../img/home-parallax-144609983.jpg);
    padding: 150px;
    background-size: cover;
    position: relative;

    .review-small-container{
        text-align: center;
        padding: 80px 0;
        color: white;

        hr{
        @include hr-base;
        }

        .account-img{
            width: 150px;
            height: 150px;
            margin: 0 auto;
            background-image: url(../img/home-testimonial-113165296.jpg);
            border-radius: 50%;
            margin-bottom: 30px;
        }
        
        p{
            margin-bottom: 50px;
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
<script>
import Jumbo from './Jumbo.vue';
import CardUno from './CardUno.vue';
import Statistics from './Statistics.vue';
import CardDue from './CardDue.vue';
import ValuesCard from './ValuesCard.vue';
import Reviews from './Reviews.vue';

export default {
name: 'MainApp',

  data () {
      return{

      }
  },

  components:{
    Jumbo,
    CardUno,
    Statistics,
    CardDue,
    ValuesCard,
    Reviews,
  },
  methods:{},

}
</script>

<template>

    <main>

      
      <!-- SEZIONE JUMBO -->
      <section>
        <Jumbo />
      </section>

      <!-- SEZIONE CARD N.1 -->
      <section>
        <div class="card-big-container">

          <h3>Specialists in Modern Costruction</h3>

          <hr>

          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nisi ducimus laudantium tenetur molestias unde modi <br>repellat maxime reiciendis quia cum?</p>

          <div class="container d-flex justify-content-between card1-small-container">

            <CardUno />

          </div>

        </div>
      </section>

      <!-- SEZIONE STATISTICHE -->
      <Statistics />

      <!-- SEZIONE CARD N.2 -->
      <section>
        <div class="card-big-container">

          <h3>Explore Recent Work</h3>

          <hr>

          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nisi ducimus laudantium tenetur molestias unde modi <br>repellat maxime reiciendis quia cum?</p>

          <div class="container d-flex justify-content-between card2-small-container">

            <CardDue />

          </div>

        </div>
      </section>

      <!-- SEZIONE VALUES -->
      <section>
        <div class="card-big-container gray">

          <h3>Our Core Values</h3>

          <hr>

          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nisi ducimus laudantium tenetur molestias unde modi <br>repellat maxime reiciendis quia cum?</p>

          <div class="container d-flex justify-content-between card2-small-container">

            <ValuesCard />

          </div>

        </div>
      </section>

      <!-- SEZIONE REVIEWS -->
      <Reviews />

        
    </main>
 
</template>

<style lang="scss">
main{
  padding-top:60px;
  background-color: white;

  //SEZIONE CARD UNO
  .card-big-container{
    text-align: center;
    padding: 80px 0;

    hr{
      @include hr-base;
    }

    .card1-small-container{
      margin-top: 80px;
    }
  }

  // SEZIONE CARD DUE
  .card2-small-container{
    margin-top: 80px;
    width: 70%;
  }

  // SEZIONE VALUES
  .gray{
    background-color: $main-white;
  }

}

</style>

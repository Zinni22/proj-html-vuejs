<script>
import Jumbo from './Jumbo.vue';
import CardUno from './CardUno.vue'

export default {
name: 'MainApp',

  data () {
      return{

      }
  },

  components:{
    Jumbo,
    CardUno,
  },
  methods:{},

}
</script>

<template>

    <main>

      <!-- SEZIONE JUMBO -->
      <Jumbo />

      <!-- SEZIONE CARD N.1 -->
      <div class="card1-big-container">

        <h3>Specialists in Modern Costruction</h3>

        <hr>

        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nisi ducimus laudantium tenetur molestias unde modi <br>repellat maxime reiciendis quia cum?</p>

        <div class="container d-flex justify-content-between card1-small-container">

          <CardUno />

        </div>

      </div>

        
    </main>
 
</template>

<style lang="scss">
main{
    padding-top:60px;
    background-color: white;

    .card1-big-container{
      text-align: center;
      padding: 80px 0;

      hr{
        @include hr-base;
      }

      .card1-small-container{
        margin-top: 80px;
      }
    }
}

</style>

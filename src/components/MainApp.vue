<script>
import Jumbo from './Jumbo.vue';

export default {
name: 'MainApp',

  data () {
      return{

      }
  },

  components:{
    Jumbo,
  },
  methods:{},

}
</script>

<template>

    <main>

        <Jumbo />

        
    </main>
 
</template>

<style lang="scss">
main{
    padding-top:60px;
}

</style>

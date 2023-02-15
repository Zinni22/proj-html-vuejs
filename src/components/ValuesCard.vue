<script>

export default {
name: 'MainApp',

  data () {
      return{

        valuesList: [
            {
                icon: ['fas', 'house'],
                title: 'Great Services',
                text: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque',
            },
            {
                icon: ['fas', 'gear'],
                title: 'Highest Standards',
                text: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque',
            },
            {
                icon: ['fas', 'users'],
                title: 'Professional Team',
                text: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque',
            },
            {
                icon: ['fas', 'lightbulb'],
                title: 'Great Services',
                text: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque',
            },

        ]

      }
  },

  components:{},
  methods:{},

}
</script>

<template>

    <div v-for="value in valuesList" class="value-card">

        <font-awesome-icon :icon="value.icon" class="icon"/>

        <p>
            <strong> {{ value.title }} </strong>
        </p>

        <hr>

        <p>
            {{ value.text }}
        </p>
        
    </div>

</template>

<style lang="scss" scoped>

.value-card{
    margin-right: 15px;

    .icon{
        background-color: $second-green;
        font-size:1.5rem;
        width: 1.5rem;
        padding: 1.5rem;
        border-radius: 50%;
        color: white;
        margin-bottom: 20px;
    }

    hr{
        background-color: black;
        height: 2px;
        width: 20%;
        margin: 15px auto;
    }
}

.value-card:hover{
    cursor: pointer;
    .icon{
        background-color: $main-yellow;
    }
    p:nth-of-type(1){
        color: $main-yellow;
    }

}

</style>
<script>

export default {
name: 'MainApp',

  data () {
      return{

        cards: [
            {
                icon: ['fas', 'building'],
                type: 'Building',
                text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Omnis necessitatibus, corrupti dignissimos ea at beatae!',
            },
            {
                icon: ['fas', 'arrows-spin'],
                type: 'Rennovate',
                text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Omnis necessitatibus, corrupti dignissimos ea at beatae!',
            },
            {
                icon: ['fas', 'house'],
                type: 'Construct',
                text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Omnis necessitatibus, corrupti dignissimos ea at beatae!',
            },
            {
                icon: ['fas', 'truck'],
                type: 'Exclusive',
                text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Omnis necessitatibus, corrupti dignissimos ea at beatae!',
            },
        ]

      }
  },

  components:{
  },
  methods:{},

}
</script>


<template>

    <div class="card-uno" v-for="card in cards">

        <font-awesome-icon :icon="card.icon" class="icon"/>

        <h4>
            {{card.type}}
        </h4>

        <p>
            {{card.text}}
        </p>

        <button>
            get a quote
        </button>

    </div>

</template>


<style lang="scss" scoped>
.card-uno{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 20px;
    width: calc(100%/4 - 20px);
    background-color: $main-white;
    border-radius: 15px;

    .icon{
        font-size: 1.5rem;
        width: 1.5rem;
        height: 1.5rem;
        padding: 1.5rem;
        border: 1px solid black;
        border-radius: 50%;
        margin-bottom: 20px;
    }

    button{
        display: none;
        @include button-base;
        background-color: rgba(255, 255, 255, 0.5);
        margin: 0 auto;
    }
}

.card-uno:hover{
    background-color: $main-yellow;
    cursor: pointer;
    transform: rotateY('180deg');

    .icon{
        display: none;
    }
    
    h4{
        text-transform: uppercase;
        margin-bottom: 20px;
    }

    button{
        display: block;
    }
}
</style>
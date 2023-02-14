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

    <!-- CONTENITORE PRINCIPALE -->
    <div class="d-flex justify-content-center align-items-center main-container">

        <!-- CONTENITORE FLEXATO -->
        <div>
            <h1>
                building inspiring spaces
            </h1>

            <p>
                We Build Inspiring Residential & Commercial Spaces
            </p>

            <div class="d-flex justify-content-center">
                <button>
                    explore recent work
                </button>

                <button>
                    get a quote today
                </button>
            </div>
        </div>

    </div>

    <!-- BANDA GIALLA -->
    <div class="yellow-question">
        Do You Have A Construction Project We Can Help With?
    </div>
 
</template>

<style lang="scss" scoped>

//CONTENITORE PRICIPALE
.main-container{
   background-image: url(../img/home-slider-62528242.jpg);
   background-size: cover;
   padding: 130px 0;

   div{
    text-align: center;

    h1{
        text-transform: uppercase;
        color: white;
        font-weight: 700;
    }

    p{
        color: $main-yellow;
    }

    div{
        button{
            @include button-base;
            margin-right: 10px;
        }
        button:nth-child(1){
            background-color: $main-gray;
            color: white;
        }
        button:nth-child(1):hover{
            background-color: $main-yellow;
            color: black;
        }
        button:nth-child(2):hover{
            background-color: $main-gray;
            color: white;
        }
    }

   }
}

//BANDA GIALLA{
.yellow-question{
    background-color: $main-yellow;
    text-align: center;
    padding: 30px 0;
}


</style>

<script>

export default {
name: 'MainApp',

  data () {
      return{

      }
  },

  components:{
  },
  methods:{},

}
</script>

<template>

    <div class="card-due">

        <div class="content-card-due">

            <div class="d-flex justify-content-center">
                <div class="icon">
                    <font-awesome-icon icon="fa-solid fa-link" />
                </div>
                <div class="icon">
                    <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
                </div>
            </div>

            <p>Florida Heath Facility</p>

            <p>Commercial</p>

        </div>

    </div>

    <div class="card-due">

        <div class="content-card-due">

            <div class="d-flex justify-content-center">
                <div class="icon">
                    <font-awesome-icon icon="fa-solid fa-link" />
                </div>
                <div class="icon">
                    <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
                </div>
            </div>

            <p>Florida Heath Facility</p>

            <p>Commercial</p>

        </div>

    </div>

    <div class="card-due">

        <div class="content-card-due">

            <div class="d-flex justify-content-center">
                <div class="icon">
                    <font-awesome-icon icon="fa-solid fa-link" />
                </div>
                <div class="icon">
                    <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
                </div>
            </div>

            <p>Florida Heath Facility</p>

            <p>Commercial</p>

        </div>

    </div>

</template>

<style lang="scss" scoped>
.card-due{
    width: 300px;
    height: 300px;
    background-size: cover;
    display: flex;
    flex-direction: column;
    justify-content: center;
    color: white;

    img{
        width: 100%;
    }

    .content-card-due{
        display: none;
        .icon{
            width: 3rem;
            height: 3rem;
            line-height: 3rem;
            text-align: center;
            background-color: white;
            color: $main-yellow;
            border-radius: 50%;
            margin: 0 10px 20px 0;
        }
    }
}
.card-due:nth-child(1){
    background-image: url("../img/project2-featured-15013609-200x200.jpg");
}
.card-due:nth-child(2){
    background-image: url("../img/project1-featured-294276386-200x200.jpg");
}
.card-due:nth-child(3){
    background-image: url("../img/project3-featured-189023420-200x200.jpg");
}

.card-due:hover{
    background-color: $main-yellow;
    background-image: none;

    .content-card-due{
        display: block;
    }
}
</style>
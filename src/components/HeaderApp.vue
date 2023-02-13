<script>
export default {
name: 'HeaderApp',

  data () {
      return{
        headerMenuList: [
            "home",
            "about",
            "services",
            "work",
            "articles"
        ]
      }
  },

  components:{},
  methods:{},

}
</script>

<template>

    <header>

        <div>
            <img src="../img/construction_logo.png" alt="header_logo">
        </div>
        
        <div>
            <ul>
                <li v-for="singleVoice in headerMenuList">
                {{ singleVoice }} 
                </li>
            </ul>
        </div>

    </header>
 
</template>

<style lang="scss" scoped>

header{
    display: flex;
    justify-content: space-between;
    height: 60px;
    background-color: red;
    div{

        img{
            height: 100%;
        }

        ul{
            display: flex;
            align-items: center;
            height: 100%;

            li{
                margin-right: 20px;
                text-transform: uppercase;
            }
        }
    }

}

</style>

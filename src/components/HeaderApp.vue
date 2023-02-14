<script>
export default {
name: 'HeaderApp',

  data () {
      return{
        headerMenuList: [
            {
                link: "#",
                voice: "home"
            },
            {
                link: "#",
                voice: "about"
            },
            {
                link: "#",
                voice: "services"
            },
            {
                link: "#",
                voice: "work"
            },
            {
                link: "#",
                voice: "articles"
            },
        ]
      }
  },

  components:{},
  methods:{},

}
</script>

<template>

    <header>

        <div class="container d-flex justify-content-between">

            <!-- LOGO -->
            <img src="../img/construction_logo.png" alt="header_logo">
        
            <!-- MENU -->
            <ul>
                <li v-for="singleVoice in headerMenuList">
                    <a :href="singleVoice.link">
                        {{ singleVoice.voice }}
                    </a>
                </li>

                <!-- BOTTONE -->
                <button>
                    get quote
                </button>
            </ul>
            
        </div>

    </header>
 
</template>

<style lang="scss">

header{
    background-color: white;
    position: fixed;
    width: 100%;
    z-index: 30;

    div{
        height: 60px;
        padding: 10px 0;

        //LOGO
        img{
            height: 100%;
        }

        //MENU
        ul{
            display: flex;
            align-items: center;
            height: 100%;

            li{
                a{
                    margin-right: 20px;
                    text-transform: uppercase;
                }
            }
            li:hover{
                a{
                    color: $main-yellow;
                }
            }

            //BOTTONE
            button{
                border: 0px;
                background-color: $main-yellow;
                padding: 2px 20px;
                cursor: pointer;
            }
            button:hover{
                background-color: $main-gray;
                color: $main-white;
            }
        }

    }

}

</style>

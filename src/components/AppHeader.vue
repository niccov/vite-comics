<script>
  export default {
    data() {
        return {
            links: [
                'characters',
                'comics',
                'movies',
                'tv',
                'games',
                'collectibles',
                'videos',
                'fans',
                'news',
                'shop'
            ],
        }
    }
  }
</script>

<template>
    <header>
       <div id="container-logo">
         <img src="dc-logo.png" alt="logo">
       </div>

       <nav>
          <ul v-for="link in links">
            <li>{{link}}</li>

          </ul>
       </nav>
    </header>   
</template>

<style lang="scss" scoped>

header{
    width: 75%;

    margin: 10px auto;

    display: flex;
    justify-content: space-between;
    align-items: center;

    #container-logo{
        height: 60px;

        img{
          height: 100%;
        }
    }

    nav{
        display: flex;

        li{
            padding: 15px 15px 20px 15px;


            &:hover{
              border-bottom: 1px solid;
              border-bottom-color: #0282F9;
              color: #0282F9;
            }
        }
    }
}
</style>
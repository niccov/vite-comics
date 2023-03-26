<script>
  export default{
    data() {
        return {
            cards: [
                {

                image: '../../public/buy-comics-digital-comics.png',
                text: 'DIGITAL COMICS '
            }, 

                {
                
                image: '../../public/buy-comics-merchandise.png',
                text: 'DC MERCHANDISE'
            },   

                {

                image: '../../public/buy-comics-subscriptions.png',
                text: 'SUBSCRIPTION'
            }, 
            
                {
                image: '../../public/buy-comics-shop-locator.png',
                text: 'COMIC SHOP LOCATOR'
            },  

                {
                image: '../../public/buy-dc-power-visa.svg',
                text: 'DC POWER VISA'
            }    
                
            ]
        }
    },

    methods: {

    }
  }
</script>

<template>
    <div id="jumbo">
        <div id="jumbo-top">
            <h2>_ _>Content goes here</h2>
        </div>
        <div id="jumbo-bottom">
            <div v-for="card in cards" id="card">
               <div id="container-img">
                  <img :src="card.image" >
                </div>  
               <div>{{ card.text }}</div>
            </div>  
        </div>
    </div>
</template>

<style lang="scss" scoped>
   #jumbo {
     height: 160px;
     #jumbo-top {
        height: 50%;

        background-color: black;

        h2 {
            color: white;

            margin-left: 150px;
            line-height: 80px;
        }
     }

     #jumbo-bottom {
        height: 50%;

        background-color: #0282F9;

        display: flex;
        justify-content: center;
        align-items: center;

        #card {
            display: flex;
            align-items: center;

            padding: 15px;

            #container-img {
        
                width: 35px;
                

                img{
                   width: 100%; 
                }
            }

            div{
                color: white;
                font-size: 14px;
                
                padding-left: 5px;
            }
        }
     }
   }
</style>
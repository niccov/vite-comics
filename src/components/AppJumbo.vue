<script>

import AppSeries from './AppSeries.vue';

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
                
            ],

            series: [
           {
             thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
             price: "$19.99",
             series: "Action Comics",
             type: "comic book"
           },
           {
             thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
             price: "$3.99",
             series: "American Vampire 1976",
             type: "comic book"
           },
           {
             thumb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
             price: "$16.99",
             series: "Aquaman",
             type: "graphic novel"
           },
           {
             thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
             price: "$2.99",
             series: "Batgirl",
             type: "comic book"
           },
           {
             thumb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
             price: "$3.99",
             series: "Batman",
             type: "comic book"
           },
           {
             thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
             price: "$2.99",
             series: "Batman Beyond",
             type: "comic book"
           },
           {
             thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
             price: "$3.99",
             series: "Batman/Superman",
             type: "comic book"
           },
           {
             thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
             price: "$4.99",
             series: "Batman/Superman Annual",
             type: "comic book"
           },
           {
             thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
             price: "$5.99",
             series: "Batman: The Joker War Zone",
             type: "comic book"
           },
           {
             thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
             price: "$6.99",
             series: "Batman: Three Jokers",
             type: "comic book"
           },
           {
             thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
             price: "$4.99",
             series: "Batman: White Knight Presents: Harley Quinn",
             type: "comic book"
           },
           {
             thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
             price: "$16.99",
             series: "Catwoman",
             type: "graphic novel"
           }
         ]
        }
    },

    components: {
        AppSeries,
    },

    methods: {

    }
  }
</script>

<template>
    <div id="jumbo">
        <div id="jumbo-img">
          <div id="titolo-jumbo"><b>CURRENT SERIES</b></div>
        </div>

        <div id="jumbo-top">
            <div id="container-series">

                <AppSeries v-for="serie in series" :img="serie.thumb" :serie="serie.series"></AppSeries>
                
            </div>   
            
            <div id="container-button">
                <button>LOAD MORE</button>
            </div>
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

     #jumbo-img{
       width: 100%;
       height: 300px;

       background-image: url(../../public/jumbotron.jpg);
       background-size: cover;

       position: relative;

       #titolo-jumbo{
        padding: 10px 30px;
        background-color: #0282F9;

        color: white;

        position: absolute;
        left: 100px;
        bottom: -20px;
       }
     }
    
     #jumbo-top {
        

        background-color: black;

        #container-series{
            width: 1200px;
            margin: auto;

            display: flex;
            flex-flow: row wrap;
            justify-content: center;
        }

        #container-button{

            text-align: center;


            button{
                background-color: #0282F9;
                padding: 5px 30px;

                border-color: #0282F9;

                color: white;

                margin-bottom: 10px;
            }
        }
     }

     #jumbo-bottom {
        

        background-color: #0282F9;

        display: flex;
        justify-content: center;
        align-items: center;

        #card {
            display: flex;
            align-items: center;

            padding: 20px;

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
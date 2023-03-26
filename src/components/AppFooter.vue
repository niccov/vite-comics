<script>

 export default {
    data() {
        return {
            
        }
    }
 }
</script>

<template>
<footer>
    <div id="top-footer">
        <div id="top-footer-links">
           <div class="column-links">
            <div>
               <h3>DC COMICS</h3>

               <ul>
                <li>Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>TV</li>
                <li>Games</li>
                <li>Videos</li>
                <li>News</li>
               </ul>
            </div>

            <div>
                <h3>SHOP</h3>

                <div>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
            </div>

           </div>

           <div class="column-links">

                <h3>DC</h3>

                <div>
                    <ul>
                        <li>Terms Of Use</li>
                        <li>Privacy policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshop</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>

           </div>

           <div class="column-links">
              <h3>SITES</h3>

              <div>
                <ul>
                    <li>DC</li>
                    <li>MAD Magazine</li>
                    <li>DC Kids</li>
                    <li>DC Universe</li>
                    <li>DC Power Visa</li>
                </ul>
              </div>
           </div>
        </div>  
        
        <div id="container-img"></div>
    </div>

    <div id="bottom-footer">
        <div id="container-bottom-footer">
            <div id="bottom-left">
                <button>SIGN-UP NOW!</button>
            </div>

            <div id="bottom-right">
                <h3>FOLLOW US</h3>
                <div id="social">
                    <div>
                        <img src="../../public/footer-facebook.png" alt="facebook">
                    </div>

                    <div>
                        <img src="../../public/footer-twitter.png" alt="twitter">
                    </div>

                    <div>
                        <img src="../../public/footer-youtube.png" alt="youtube">
                    </div>

                    <div>
                        <img src="../../public/footer-pinterest.png" alt="pinterest">
                    </div>

                    <div>
                        <img src="../../public/footer-periscope.png" alt="periscope">
                    </div>
                </div>
            </div>
        </div>
    </div>
</footer>
</template>

<style lang="scss" scoped>

  footer{
    color: white;
  }

  #top-footer {
    height: 335px;
    
    background-image: url(../../public/footer-bg.jpg);

    display: flex;
    gap: 30px;


    #top-footer-links{

        margin-left: 250px;

        display: flex;

      .column-links {
        padding: 20px 15px;

        h3{
            margin-top: 10px;
        }
        
        ul {


          li {
            font-size: 14px;
            color: grey;
          }
        }  
      }
    }  

    #container-img {
        height: 100%;
        width: 500px;

        background-image: url(../../public/dc-logo-bg.png);

        background-size: cover;

        background-position: center;
    }
  }

  #bottom-footer {
    height: 80px;

    background-color: #303030;

    #container-bottom-footer {

        height: 100%;
        width: 65%;
        margin: auto;

        display: flex;
        align-items: center;
        justify-content: space-between;
        
        #bottom-left {
            button {
                padding: 10px 10px;

                border-color: #0282F9;

                background-color: #303030;

                color: white;
            }
        }

        #bottom-right{
            display: flex;
            align-items: center;
            gap: 10px;

            h3{
                color: #0282F9;
            }

            #social{
                display: flex;
                align-items: center;
                gap: 10px;
            }
        }
    }
  }

</style>
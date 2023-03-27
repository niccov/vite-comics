<script>

export default {
    name: "AppSeries",

    data() {

    },

    props: {
        img: String,

        serie: String,
    }
}
</script>

<template>
    <div class="serie">
        <div class="container-img">
            <img :src="img" alt="">
        </div>

        <div class="titol">
            <h3>{{serie}}</h3>
        </div>
    </div>
</template>

<style lang="scss" scoped>

.serie {
    padding: 30px 15px 15px 15px;

    width: calc(100% / 6);
    
    .container-img{
        width: 150px;
        height: 150px;
        

        img {
            width: 100%;  
            height: 100%;

            object-fit: cover;
        }
    }

    .titol{
        h3{
            color: white;

            font-size: 14px;
        }
    }


}

</style>
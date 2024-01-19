<script>
export default {
    data() {
        return {

        };
    },
    props: {
        comic: Object
    }
}
</script>

<template>

        <div class="item-comic-container">
            <div class="comic-container">
                <img :src="comic.thumb" :alt="comic.series">
            </div>
            <h3>
                {{comic.series}}
            </h3>
        </div>

</template>

<style lang="scss" scoped>
    @use "../assets/scss/partials/variables.scss" as *;
    @use "../assets/scss/partials/mixins.scss" as *;

    .item-comic-container{
        width: calc((100% / 6) - 30px);
        margin: 0 $spacing_15;
        margin-bottom: $spacing_30;

        .comic-container{
            width:$percent_100;
            height: 137px;

            img{
                width: $percent_100;
                object-fit: cover;
                object-position: top center;
                height: 100%;
            }
        }

        h3{
            color: $white_color;
            margin-top: $spacing_15;
            font-size: $font_size_small;
            text-transform: uppercase;
        }

    }
    
</style>



        
    


                

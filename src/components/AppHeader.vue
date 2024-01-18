<script>
export default {
    data() {
        return {
            navbar : [
                {
                    item: 'CHARACTERS'
                },
                {
                    item: 'COMICS'
                },
                {
                    item: 'MOVIES'
                },
                {
                    item: 'TV'
                },
                {
                    item: 'GAMES'
                },
                {
                    item: 'COLLECTIBLES'
                },
                {
                    item: 'VIDEOS'
                },
                {
                    item: 'FANS'
                },
                {
                    item: 'NEWS'
                },
                {
                    item: 'SHOP'
                }
            ]
        };
    },
    methods: {

    }
}
</script>

<template>
    <header>
        <div>
            <div>
                <img src="../../public/vue-dc-comics-1/img/dc-logo.png" alt="Logo DC">
            </div>
            
            <nav>
                <ul>
                    <li v-for="(singleItem, i) in navbar">{{ singleItem.item }}</li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
    @use "../assets/scss/partials/variables.scss" as *;
    @use "../assets/scss/partials/mixins.scss" as *;

    header{
        padding: $spacing_20;
        background-color: $white_color;
        >div{
            @include container;
            @include row;
            justify-content: $space_between;
            align-items: $XY_flex_center;
            
            div{
                width: $logo_dimension;
                height: $logo_dimension;
                margin-right: $spacing_50;

                img{
                    width: $percent_100;
                    display: block;
                }
            }
        }

        ul{
            li{
                display: inline-block;
                padding: 0 $spacing_10;
                font-size: $font_size_small;
                font-weight: $font_bold;
                color: $dark_gray_color;

                &:hover{
                    color: $blue_brand;
                    cursor: pointer;
                }
            }
        }
            

    }
</style>

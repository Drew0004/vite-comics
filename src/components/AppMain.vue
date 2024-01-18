<script>
export default {
    data() {
        return {
            blueItems : [
                {
                    image: '../../public/vue-dc-comics-1/img/buy-comics-digital-comics.png',
                    caption: 'DIGITAL COMICS'
                },
                {
                    image: '../../public/vue-dc-comics-1/img/buy-comics-merchandise.png',
                    caption: 'DC MERCHANDISE'
                },
                {
                    image: '../../public/vue-dc-comics-1/img/buy-comics-subscriptions.png',
                    caption: 'SUBSCRIPTION'
                },
                {
                    image: '../../public/vue-dc-comics-1/img/buy-comics-shop-locator.png',
                    caption: 'COMIC SHOP LOCATOR'
                },
                {
                    image: '../../public/vue-dc-comics-1/img/buy-dc-power-visa.svg',
                    caption: 'DC POWER VISA'
                },
            ]

        };
    },
    methods: {

    }
}
</script>

<template>
    <main>
        <section class="main-gray">
            <div>
                <h2>Content goes here </h2>
            </div>
        </section>

        <section class="blue-main">
            <div>
                content
            </div>
        </section>


    </main>
</template>

<style lang="scss" scoped>
    @use "../assets/scss/partials/variables.scss" as *;
    @use "../assets/scss/partials/mixins.scss" as *;
    
    main{
        .main-gray{
            background-color: $main_background_color;
            padding: $spacing_50;
        
            >div{
                @include container;

                h2{
                    font-size: $font_size_large;
                    font-weight: $font_bold;
                    color: $white_color;
                }
            }
        }

        .blue-main{
            background-color: $blue_brand;
            padding: $spacing_50;
            
            >div{
                @include container;
            }
        }
        
    
    }

</style>

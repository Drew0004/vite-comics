<script>
export default {
    data() {
        return {
            dcComics: [
                {
                    title: 'Characters'
                },
                {
                    title: 'Comics'
                },
                {
                    title: 'Movies'
                },
                {
                    title: 'TV'
                },
                {
                    title: 'Games'
                },
                {
                    title: 'Videos'
                },
                {
                    title: 'News'
                },
            ],
            shop: [
               {
                    title: 'Shop DC'
                }, 
                {
                    title: 'Shop DC Collectibles'
                },
            ],
            dc: [
                {
                    title:'Terms of use'
                },
                {
                    title:'Privacy policy (New)'
                },
                {
                    title:'Ad Choices'
                },
                {
                    title:'Advertising'
                },
                {
                    title:'Jobs'
                },
                {
                    title:'Subscriptions'
                },
                {
                    title:'Talent Workshops'
                },
                {
                    title:'CPSC Certificates'
                },
                {
                    title:'Ratings'
                },
                {
                    title:'Shop Help'
                },
                {
                    title:'Contact Us'
                },
            ],
            sites: [
                {
                    title:'DC'
                },
                {
                    title:'MAD Magazin'
                },
                {
                    title:'DC Kids'
                },
                {
                    title:'DC Universe'
                },
                {
                    title:'DC Power Visa'
                },
            ]

        };
    },
    methods: {

    }
}
</script>

<template>
    <footer>
        
        <section class="upper-foot">
            
            <div class="foot-img-container">
            
                <div>
                    
                    <div class="foot-list">
                        <h3>DC COMICS</h3>
                        <ul>
                            <li v-for="(singleElem, i) in dcComics"> {{ singleElem.title }}</li>
                        </ul>
                        
                        <h3>SHOP</h3>
                        <ul>
                            <li v-for="(singleElem, j) in shop">{{ singleElem.title }}</li>
                        </ul>
                    </div>
                
                    <div class="foot-list">
                        <h3>DC</h3>
                        <ul>
                            <li v-for="(singleElem, z) in dc">{{ singleElem.title }}</li>
                        </ul>
                    </div>
                    
                    <div class="foot-list">
                        <h3>Sites</h3>
                        <ul>
                            <li v-for="(singleElem, x) in sites">{{ singleElem.title }}</li>
                        </ul>
                    </div>

                    <div class="overflow-logo">
                        <img src="../../public/vue-dc-comics-1/img/dc-logo-bg.png" alt="Logo Background">
                    </div>

                </div>

            </div>  
        
        </section>

        <section class="lower-foot">
            <div>
                <div>
                    <button class="foot-button">
                        SIGN UP NOW!
                    </button>
                </div>
                
                <div class="lower-foot-icon">
                    <h2>FOLLOW US</h2>
                    <ul>
                        <li><img src="../../public/vue-dc-comics-1/img/footer-facebook.png" alt="Facebook icon"></li>
                        <li><img src="../../public/vue-dc-comics-1/img/footer-twitter.png" alt="Twitter icon"></li>
                        <li><img src="../../public/vue-dc-comics-1/img/footer-youtube.png" alt="Youtube icon"></li>
                        <li><img src="../../public/vue-dc-comics-1/img/footer-pinterest.png" alt="Pinterest icon"></li>
                        <li><img src="../../public/vue-dc-comics-1/img/footer-periscope.png" alt="Periscope icon"></li>
                    </ul>
                </div>
            </div>
        </section>
    
    </footer>
</template>

<style lang="scss" scoped>
    @use "../assets/scss/partials/variables.scss" as *;
    @use "../assets/scss/partials/mixins.scss" as *;

    .foot-img-container{
        @include foot-box-img;

        >div{
            @include container;
            @include row;
            justify-content: space-between;
        }

        .foot-list{
                margin-right: $spacing_20;
                margin-top: $spacing_20;

                li{
                    color: gray;
                    cursor: pointer;
                    padding-bottom: $spacing_10;
                    font-size: $font_size_small;
                }
                
                h3{
                    margin: $spacing_20 0;
                    color: $white_color;
                }
        }

        .overflow-logo{
            overflow: hidden;
            display: flex;
            align-items: center;
            height: 400px;
             
                img{
                    height: 150%;
                    display: block;
                }
        }
    }

    .lower-foot{
        padding: $spacing_30;
        background-color: $footer_gray_color;

        >div{
            @include container;
            @include row;
            justify-content: $space_between;
            align-items: $XY_flex_center;
        }

        .foot-button{
            background-color: $footer_gray_color;
            border: 2px solid $blue_brand;
            font-size: $font_size_mid;
            color: $white_color;
            padding: $spacing_10;
        }

        .lower-foot-icon{
            @include row;
            @include flex_center;
                
                h2{
                    margin-right: $spacing_20;
                    color: $blue_brand;
                }

                li{
                    display: inline-block;
                    padding: 0 $spacing_10;
                }
        }
    }
</style>



<script>
export default {
    data() {
        return {

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
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        
                        <h3>SHOP</h3>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                
                    <div class="foot-list">
                        <h3>DC</h3>
                        <ul>
                            <li>Terms of Use</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>
                    
                    <div class="foot-list">
                        <h3>Sites</h3>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>

                    <div class="overflow-logo">
                        <img src="../../public/vue-dc-comics-1/img/dc-logo-bg.png" alt="Logo Background">
                    </div>

                </div>

            </div>  
        
        </section>

        <section>
            Lower foot
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
</style>



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
    <main>
        <div>
            <h2>Content goes here </h2>
        </div>
    </main>
</template>

<style lang="scss" scoped>
    @use "../assets/scss/partials/variables.scss" as *;
    @use "../assets/scss/partials/mixins.scss" as *;
    
    main{
        background-color: $main_background_color;
        padding: $spacing_50;
        
        div{
            @include container;

            h2{
                font-size: $font_size_large;
                font-weight: $font_bold;
                color: $white_color;
            }
        }
    }
</style>

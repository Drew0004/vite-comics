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
        <img src="../../public/vue-dc-comics-1/img/dc-logo.png" alt="Logo DC">
        <nav>
            <ul>
                <li v-for="(singleItem, i) in navbar">{{ singleItem.item }}</li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
</style>

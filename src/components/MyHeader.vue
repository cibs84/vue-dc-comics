<template>
    <header class="container">
        <!-- Header - Logo -->
        <div class="logo">
            <a href="#">
                <img src="../assets/img/dc-logo.png" alt="DC Logo">
            </a>
        </div>

        <!-- Header - Main Menu -->
        <nav>
            <ul class="main-menu">
                <li v-for='link, index in menuLinks' :key="index">
                    <!-- <a :href="link.url" :class="{ 'current': link.current }">{{link.text}}</a> -->
                    <a :href="link.url" :class="{ 'current': index === menuItemActive }" @click="setActiveMenuItem(index)">{{link.text}}</a>
                </li> 
            </ul>
        </nav>
    </header>
</template>


<script>
export default {
    name: 'MyHeader',
    data() {
        return {
            menuItemActive: 0,
            menuLinks: [
                {
                    text: 'Characters',
                    url: '#',
                },
                {
                    text: 'Comics',
                    url: '#',
                },
                {
                    text: 'Movies',
                    url: '#',
                },
                {
                    text: 'Tv',
                    url: '#',
                },
                {
                    text: 'Games',
                    url: '#',
                },
                {
                    text: 'Collectibles',
                    url: '#',
                },
                {
                    text: 'Videos',
                    url: '#',
                },
                {
                    text: 'Fans',
                    url: '#',
                },
                {
                    text: 'News',
                    url: '#',
                },
                {
                    text: 'Shop',
                    url: '#',
                }
            ]
        }
    },
    methods: {
        setActiveMenuItem(index) {
            this.menuItemActive = index;
        }
    }
}
</script>


<style lang="scss" scoped>
@import '../styles/variables';

header {
    display: flex;
    justify-content: space-between;
    align-items: center;

    .logo {
        width: 5rem;
        flex-shrink: 0;
    }
    .main-menu {
        display: flex;

        li {
            margin-left: 2rem;

            a {
                padding: 3rem 0;
                display: block;
                text-transform: uppercase;
                font-size: 0.85rem;
                font-weight: 700;

                &.current {
                    color: #0282f9;
                    border-bottom: 5px solid $brand_primary_color;
                }
            }
        }

    }
}
</style>
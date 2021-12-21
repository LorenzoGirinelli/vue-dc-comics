<template>
    <header class="container">
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="logo">
        </div>

        <nav>
            <ul class="menu">
                <li v-for="(link, index) in links" :key"index" :class="{ current: link.current }">
                    <a :href="link.url">{{ link.text }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: "Header",
    data: function () {
        return {
            links: [
                {
                    text: 'Prodotti',
                    url: '#',
                    current: false
                },
                {
                    text: 'Prodotti',
                    url: '#',
                    current: true
                },
                {
                    text: 'Prodotti',
                    url: '#',
                    current: false
                },
                {
                    text: 'Prodotti',
                    url: '#',
                    current: false
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../style/variables';
header {
    height: 150px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: aqua;
    .logo {
        img{
            width: 85px;
        }
    }
    .menu {
        display: flex;
        list-style-type: none;
        justify-content: center;
        li{
            padding: 0 10px;
            font-size: 13px;
        }
        a {
            text-decoration: none;
            font-weight: bold;
            color: #535759;
        }
        a:hover{
            color: #0282f9;
            padding-bottom: 63px;
            border-bottom: 5px solid #0282f9;
        }
    }
}
</style>

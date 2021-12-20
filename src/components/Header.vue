<template>
    <header class="container">
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="logo">
        </div>

        <nav>
            <ul class="menu">
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                                <li>
                    <a href="#">COMICS</a>
                </li>
                                <li>
                    <a href="#">MOVIES</a>
                </li>
                                <li>
                    <a href="#">TV</a>
                </li>
                                <li>
                    <a href="#">GAMES</a>
                </li>
                                <li>
                    <a href="#">COLLECTIBLES</a>
                </li>                
                <li>
                    <a href="#">VIDEOS</a>
                </li>
                <li>
                    <a href="#">FANS</a>
                </li>
                <li>
                    <a href="#">NEWS</a>
                </li>
                <li>
                    <a href="#">SHOP</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: "Header"
}
</script>

<style scoped lang="scss">
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

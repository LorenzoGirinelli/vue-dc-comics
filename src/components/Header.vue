<template>
    <header>
        <div class="container">

                <!-- logo  -->
                <div class="logo">
                    <img src="../assets/img/dc-logo.png" alt="Logo dc">
                </div>

                <!-- Menu  -->
                <div class="header-menu">
                    <ul>
                        <li 
                            v-for="(link, index) in links" 
                            :key="index"
                            :class="{ active: link.active }"
                        >
                            <a :href="link.href">{{ link.text }}</a>
                        </li>
                    </ul>
                </div>

            </div>
    </header>
</template>

<script>
export default {
    name: "Header",
    data: function() {
        return {
            links: [
                {
                    href: '#',
                    text: 'characters',
                    active: false,
                },
                {
                    href: '#',
                    text: 'comics',
                    active: true,
                },
                {
                    href: '#',
                    text: 'movies',
                    active: false,
                },
                {
                    href: '#',
                    text: 'tv',
                    active: false,
                },
                {
                    href: '#',
                    text: 'games',
                    active: false,
                },
                {
                    href: '#',
                    text: 'collectibles',
                    active: false,
                },
                {
                    href: '#',
                    text: 'videos',
                    active: false,
                },
                {
                    href: '#',
                    text: 'fans',
                    active: false,
                },
                {
                    href: '#',
                    text: 'news',
                    active: false,
                },
                {
                    href: '#',
                    text: 'shop',
                    active: false,
                },
            ],
        }
    },
}
</script>

<style lang="scss" scoped>
@import '../style/variables';
header {
    width: 100%;
    height: 120px;
    .container {
            padding: 0 20px;
            display: flex;
            justify-content: space-between;
            .logo {
                max-width: 90px;
                vertical-align: middle;
                img {
                    margin-top: 10px;
                }
            }
            .header-menu {
                li {
                    display: inline-block;
                    line-height: 110px;
                    margin: 0 12px;
                    font-size: 14px;
                    text-transform: uppercase;
                    font-weight: bold;
                    color: #535759;
                    &.active {
                        border-bottom: 5px solid $brand_primary_color;
                        color: $brand_primary_color;
                    }
                }
                a {
                    text-decoration: none;
                    font-weight: bold;
                    color: #535759;
                }
            }
        }
}
</style> 

// <style scoped lang="scss">
// header {
//     height: 150px;
//     display: flex;
//     justify-content: space-between;
//     align-items: center;
//     background-color: aqua;
//     .logo {
//         img{
//             width: 85px;
//         }
//     }
//     .menu {
//         display: flex;
//         list-style-type: none;
//         justify-content: center;
//         li{
//             padding: 0 10px;
//             font-size: 13px;
//         }
        // a {
        //     text-decoration: none;
        //     font-weight: bold;
        //     color: #535759;
        // }
//         a:hover{
//             color: #0282f9;
//             padding-bottom: 63px;
//             border-bottom: 5px solid #0282f9;
//         }
//     }
// }
// </style>

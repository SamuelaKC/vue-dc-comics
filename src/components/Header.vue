<template>
<div class="container">
    <div class="header-total">
        <div class="logo">
            <img src="../assets/dc-logo.png" alt="">
        </div>
        <nav>
            <ul>
                <li><a href="#">CHARACTERS</a></li>
                <li><a href="#">COMICS</a></li>
                <li><a href="#">MOVIES</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">GAMES</a></li>
                <li><a href="#">COLLECTIBLES</a></li>
                <li><a href="#">VIDEOS</a></li>
                <li><a href="#">FANS</a></li>
                <li><a href="#">NEWS</a></li>
                <li><a href="#">SHOP</a></li>
            </ul>
        </nav>
    </div>
</div>
</template>


<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss" scoped>
    @import "../style/colors.scss";
    @import "../style/fonts.scss";

    .header-total {
        margin-top: 50px;
        display: flex;

        .logo{
            width: 40%;
            text-align: center;
            }
        nav {
            flex-grow: 1;
            display: flex;

            ul {
                display: flex;
                list-style: none;
                justify-content: center;
                font-size: 14px;
                font-weight: bold;

                li {
                    height: 50px;
                    line-height: 50px;
                    padding: 0 10px;
                    
                    a {
                        color: #333;
                        text-decoration: none;
                        &:hover {
                            color: $link-color;
                        } 
                    }
                }
            }
        }
    }

</style>
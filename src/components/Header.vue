<template>
<div class="container">
    <div class="content">
        <div class="logo">
            <img src="../assets/dc-logo.png" alt="">
        </div>
        <div class="navbar">
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
        </div>
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

.content {
    margin-top: 50px;
    margin-bottom: 10px; 


        .logo{
            width: 40%;
            text-align: center;
            }

        .navbar {
            flex-grow: 1;
            display: flex;


            ul {
                display: flex;
                list-style: none;
                justify-content: center;
                font-size: 14px;
                font-weight: bold;

                li {
                    padding: 0 10px;
                    
                    a {
                        color: #333;
                        text-decoration: none;
                        &:hover {
                            color: $link-color;
                            padding-bottom: 50px;
                            border-bottom: 5px solid #0282f9;
                        } 
                    }
                }
            }
        }
}
</style>
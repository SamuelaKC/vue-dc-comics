<template>
<div class="container">
    <div class="content">
        <div class="navbar">
                <div class="container-link"><a href="#"><div class="container-image"><img src="../assets/buy-comics-digital-comics.png" alt="DIGITAL COMICS"></div><div class="container-text">DIGITAL COMICS</div></a></div>
                <div class="container-link"><a href="#"><div class="container-image"><img src="../assets/buy-comics-merchandise.png" alt="DC MERCHANDISE"></div><div class="container-text">DC MERCHANDISE</div></a></div>
                <div class="container-link"><a href="#"><div class="container-image"><img src="../assets/buy-comics-subscriptions.png" alt="SUBSCRIPTION"></div><div class="container-text">SUBSCRIPTION</div></a></div>
                <div class="container-link"><a href="#"><div class="container-image"><img src="../assets/buy-comics-shop-locator.png" alt="COMIC SHOP LOCATOR"></div><div class="container-text">COMIC SHOP LOCATOR</div></a></div>
                <div class="container-link"><a href="#"><div class="container-image"><img src="../assets/buy-dc-power-visa.svg" alt="DC POWER VISA"></div><div class="container-text">DC POWER VISA</div></a></div>
        </div>
        </div>
        </div>
    
</template>


<script>
export default {
    name: 'MainSectionBlue'
}
</script>

<style lang="scss" scoped>
    @import "../style/colors.scss";
    @import "../style/fonts.scss";

        .content {
        background-color: $bg-color-blue;
        color: $bg-font-color;
        font-weight: 700;
        font-size: 20px;
        height: 200px;

                .navbar {
            display: flex;


            .container-link {
                display: flex;
                justify-content: space-between;
                font-size: 14px;
                padding: 0 10px;
                    
                    a {
                        color: $bg-font-color;
                        text-decoration: none;
                    }
                    
                    .container-image {
                        // justify-content: center;
                        // align-items: center;
                        width: 30px;

                        img {
                            width: 100%;
                        }
                    };
            }
        }


        }

</style>
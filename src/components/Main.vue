<template>
<div class="container">
    <div class="content"> --> Content goes here </div></div>
    
</template>


<script>
export default {
    name: 'Main'
}
</script>

<style lang="scss" scoped>
    @import "../style/colors.scss";
    @import "../style/fonts.scss";

    .content {
        background-color: $bg-color;
        color: $bg-font-color;
        font-weight: 700;
        font-size: 20px;
    }

</style>
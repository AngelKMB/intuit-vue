<template>
    <div class="social-media">
        <p>Share my results</p>
        <div class="icons">
            <img alt="Quickbooks logo" width="155px" src="@/assets/social-icons.png">  
        </div>
    </div>
</template>

<script>
export default {
    name: 'SocialMediaIcons'
}
</script>

<style scoped>

.icons {
    display: flex;
    margin-left: 75px;
}

.icons img {
    transform: scale(2);
}

p {
    margin: revert;
    font-size: 12px;
    font-weight: 200;
}


</style>
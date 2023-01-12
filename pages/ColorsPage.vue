<template>
    <div>
        <h1 class="heading">Colors</h1>
        <BrandColors></BrandColors>

    </div>
</template>

<script>
import BrandColors from "../components/BrandColors.vue"

export default {
    components: {
        BrandColors
    }
}
</script>

<style lang="scss">
.heading {
    text-align: center;
    font-size: 2rem;
    color: #555;
    margin: 2rem auto;
    }
</style>
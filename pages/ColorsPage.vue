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
    },
    head: {
    titleTemplate: '%s | Colors',
    meta: [
      { hid: 'description', name: 'description', content: 'Workbench brand colors and their specifications' },
    ],
  }
}
</script>

<style lang="scss" scoped>
.heading {
    text-align: center;
    font-size: 2rem;
    color: #555;
    margin: 2rem auto;
    }
</style>
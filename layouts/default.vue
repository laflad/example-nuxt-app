<template>
    <div>
      <MainHeader />
      <div class="container-lg">
        <Nuxt />
        </div>
      <MainFooter />
    </div>
</template>

<script>
export default {
  components: true,
  head: {
    title: 'Workbench Brand',
    meta: [
      { charset: 'utf-8' },
      { name: 'viewport', content: 'width=device-width, initial-scale=1' },
      { hid: 'Workbench Brand Site', name: 'Workbench Brand', content: 'Workbench brand guidelines' },
      { name: 'format-detection', content: 'telephone=no' }
    ],
  }
}
</script>

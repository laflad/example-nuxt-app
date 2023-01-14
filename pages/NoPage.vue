<template>
    <!-- created simple 404 page -->
    <div class="nopage text-center align-middle">
        <h1>Uh oh!</h1>
        <p>You landed a page that does not exist. Please select another page. Thanks!</p>
    </div>
</template>

<script>
export default {
    head: {
    titleTemplate: '%s | 404',
    meta: [
      { hid: 'description', name: 'description', content: 'Page not found' },
    ],
  }
}
</script>

<style lang="scss" scoped>
.nopage {
    padding-top: 4rem;
    color: #006887;
}

</style>
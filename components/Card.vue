<template>
    <div class="cardeffect">
        <article class="card">
            <img :src="country.flag" :alt="country.name" class="card__img">
            <h2 class="card__title">{{ country.name }}</h2>
            <p class="card__copy">{{ country.subregion }}</p>
        </article>
    </div>
</template>

<script>
export default {
    props: {
        country: Object
    }
}
</script>

<style lang="scss">
.card {
    margin: 1rem;
    border-radius: 5px;
    padding: 1.5rem;
    border: none;
    max-width: 200px;
    min-height: 250px;
    box-shadow: rgba(0, 0, 0, 0.2) 0px 18px 50px -10px;
    transition: transform 3s ease;
    &__img {
        display: block;
        margin-bottom: 1rem;
    }
    &__title {
        font-size: 1rem;
        margin-bottom: .25rem;
    }
    &__copy {
        font-size: .875rem;
    }
}

.cardeffect:hover {
    scale: (1.05);
}

.cardeffect {
    transition: 0.2s ease;
}
</style>
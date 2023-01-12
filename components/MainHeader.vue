<template>
    <div class="container-lg">
        <h1 class="maintitle">Project Workbench</h1>
        <nav class="topnav">
            <ul>
                <li><NuxtLink to="/accordions">Accordions</NuxtLink></li>
                <li><NuxtLink to="/ColorsPage">Colors</NuxtLink></li>
                <li><NuxtLink to="/flags">Countries</NuxtLink></li>
                <li><NuxtLink to="/HomePage">Home</NuxtLink></li>
            </ul>
        </nav>
    </div>

</template>

<script>
export default {
    components: true
}

</script>

<style lang="scss">
.maintitle {
    color: #006887;
    font-weight: bolder;
}

.topnav {
    overflow: hidden;
    background-color: #1e2829;
    color: white;
    border-radius: 7px;
    ul {
        list-style: none;
    }
    a {
        float: right;
        color: white;
        text-align: center;
        padding: 20px 30px;
        text-decoration: none;
        font-size: 15px;
        transition: 300ms ease;
    }
    a:hover {
        background-color: #8cd7ed;
        color: #1e2829;
    }
    a.active {
        background-color: #006887;
        color: white;
        font-weight: bold;
    }
    .nuxt-link-exact-active {
        background-color: #006887;
    }
}
</style>
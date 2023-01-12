<template>
    <footer class="row footer">
        <div class="container-lg cats">
            <div class="footerleft">
                <img class="esveegee" src="../assets/hammer-icon.svg" alt="hammer icon">
                <p>2023 Workbench | Seattle, WA<br>This website is for a class project only.</p>
            </div>
            <div class="footercenter">
                <a href="https://www.apple.com/app-store/" target="_blank">
                    <img src="../assets/ios.png" alt="apple store icon">
                </a>
                <br>
                <a href="https://play.google.com/store" target="_blank">
                    <img src="../assets/google.png" alt="google play store">
                </a>
            </div>
            <nav class="footerright">
                <ul>
                    <li><NuxtLink to="/NoPage">Help Center</NuxtLink></li>
                    <li><NuxtLink to="/NoPage">Contact Us</NuxtLink></li>
                    <li><NuxtLink to="/NoPage">Community</NuxtLink></li>
                    <li><NuxtLink to="/NoPage">Downloads</NuxtLink></li>
                </ul>
            </nav>
        </div>
    </footer>
</template>

<script>
export default {
    components: true
}

</script>

<style lang="scss">
.footer {
    position: fixed;
    bottom: 0;
    width: 100%;
    z-index: 99 !important;
    margin: 0;
    padding-top: 1rem;
    background-color: #dce4e6;
}

.cats {
    display: flex;
    flex-direction: row;
    gap: 2rem;
    justify-content: space-between;
}

.footerleft {
    font-size: small;
    width: 400px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    .esveegee {
        height: 40px;
        float: left;
        padding-right: 1rem;
    }
}

.footercenter {
    img {
        height: 30px;
        object-position: center;
        margin: 1px;
    }
}

.footerright {
    text-align: right;
    padding-right: 2rem;
    line-height: 18px;
    ul {
        list-style: none;
    }
}
</style>
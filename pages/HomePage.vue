<template>
    <div>
        <!-- simple landing page using flex grid to create side by side compartments for visuals -->
        <h3 class="apptagline">The number one rated DIY community app!</h3>
        <div class="landingpage">
            <div class="homeleft">
                <img class="splashimage" src="../assets/splash-page.png" alt="image of app">
            </div>
            <div class="homeright">
                <a href="https://www.apple.com/app-store/" target="_blank">
                    <img class="appimages" src="../assets/ios.png" alt="apple store icon">
                </a>
                <a href="https://play.google.com/store" target="_blank">
                    <img class="appimages" src="../assets/google.png" alt="google play store">
                </a>
            </div>
        </div>
    </div>
</template>

<script>

</script>

<style lang="scss">
.apptagline {
    padding-top: 2rem;
    display: flex;
    justify-content: center;
    color: #006887;
}

.landingpage {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: 1fr;
    grid-column-gap: 0px;
    grid-row-gap: 0px;
    padding-top: 4rem;
    }    

.homeleft {
    display: flex;
    flex-direction: column;
    align-items: flex-end;
}

.homeright {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    padding: 2rem;
}

.splashimage {
    height: 400px;
}

.appimages {
    width: 250px;
    padding: 1rem;
}
</style>
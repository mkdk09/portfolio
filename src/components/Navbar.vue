<template>
    <div>
        <nav class="navbar navbar-expand  navbar-dark bg-dark fixed-top">
            <div class="collapse navbar-collapse justify-content-center custom-nav" id="navbarSupportedContent">
                <div class="navbar-nav">
                    <a v-scroll-to="'#top'">TOP</a>
                    <a v-scroll-to="'#profile'">PROFILE</a>
                    <a v-scroll-to="'#skill'">SKILL</a>
                    <a v-scroll-to="'#works'">WORKS</a>
                </div>
            </div>
        </nav>
    </div>
</template>

<style scoped>
.navbar {
    height: 40px;
    filter: drop-shadow(0 5px 10px rgba(0, 0, 0, 0.6));
}

.custom-nav {
    overflow-x: scroll;
    overflow-y: hidden;
    flex-wrap: nowrap;
}

.navbar-nav {
    height: 40px;
    color: aliceblue;
}

.navbar-nav a {
    width: 100px;
    padding-top: 9px;
    padding-bottom: 10px;
}
.navbar-nav a:hover {
    background-color: darkgray;
}
</style>
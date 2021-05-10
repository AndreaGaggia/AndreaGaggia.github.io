<template>
    <nav class="shadow-2xl bg-gray-300">
        <div class="container p-2 flex justify-between items-center">
            <router-link class="avatar rounded-full" :to="{ name: 'Home' }"></router-link>
            <div class="hidden links sm:flex space-x-4">
                <router-link :to="{ name: 'About' }">About me</router-link>
                <router-link :to="{ name: 'About' }">About me</router-link>
            </div>
            <div class="sm:hidden">menu ham</div>
        </div>
    </nav>
    <router-view />
</template>

<script>
import "@lottiefiles/lottie-player";

export default {};
</script>

<style>
#app {
    min-height: 100vh;
    display: grid;
    grid-template-rows: auto 1fr;
}

a.avatar {
    width: 60px;
    height: 60px;
    background-image: url("/src/assets/avatar.svg");
    background-size: 100%;
    background-repeat: no-repeat;
    transition: 0.4s ease;
}
a.avatar:hover {
    background-color: white;
}

.links a {
    transition: 0.2s;
    position: relative;
}
.links a::after {
    content: "";
    position: absolute;
    width: 0%;
    height: 5px;
    top: 100%;
    left: 0;
    background-color: crimson;
}
.links a:hover {
    color: crimson;
}
.links a:hover::after {
    width: 50%;
    transition: width 0.2s;
}
</style>

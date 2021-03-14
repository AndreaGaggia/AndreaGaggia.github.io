<template>
    <div class="home">
        <h1>Ciao</h1>
        <iframe
            width="560"
            height="315"
            src="https://www.youtube.com/embed/lVQMyoio598?controls=0&autoplay=1&loop=1"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
        ></iframe>
    </div>
</template>

<script>
export default {
    name: "Home",
    components: {},
};
</script>

<style lang="scss" scoped>
iframe {
    border-radius: 8px;
    box-shadow: 8px 8px crimson;
}
</style>

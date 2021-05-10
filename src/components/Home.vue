<template>
    <main>
        <div>
            <lottie-player
                src="https://assets10.lottiefiles.com/packages/lf20_m6cuL6.json"
                background="transparent"
                speed="1"
                loop
                autoplay
            ></lottie-player>
        </div>
    </main>
</template>

<script>
export default {};
</script>

<style scoped>
main {
    display: grid;
    place-items: center;
}
main > div {
    height: 100%;
    min-width: 350px;
}
</style>

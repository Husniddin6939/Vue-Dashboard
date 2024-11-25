<template>
    <Header/>
    <main>
        <Navigation/>
        <section id="routing">
            <router-view></router-view>
        </section>
    </main>
    <Footer/>
</template>

<script setup>
import Header from "../../components/header/index.vue";
import Footer from "../../components/footer/index.vue";
import Navigation from "../../components/navigation/index.vue";
</script>

<style lang="scss" scoped src="./_style.scss">

</style>
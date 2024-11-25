<template>
    <aside>
        <div class="logo">
            <img src="../../assets/icons/dash.svg" alt="icon">
            <h1 href="#">Dashboard</h1>
        </div>
        <ul class="list" v-if="navlinks.length">
            <li class="list-item" v-for="el in navlinks">
                <router-link class="list-item-link" :to="el.path">
                <div v-html="el.icon"></div>
                      <span>{{ el.title }}</span>
                </router-link>
            </li>
        </ul>
    </aside>
</template>

<script setup>
import { navlinks } from '@/constants/index.js';
</script>

<style lang="scss" scoped src="./_style.scss">

</style>
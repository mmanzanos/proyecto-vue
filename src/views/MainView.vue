<template>
    <div class="container">
        <!-- Importamos el componente Sidebar.vue -->
        <Sidebar></Sidebar>
        <div class="content">
            <!-- Router-view: Al hacer clic, mostrará el componente correspondiente de cada seccion -->
            <router-view></router-view>
        </div>
    </div>
</template>

<script setup>
import Sidebar from '../components/Sidebar.vue';
</script>

<style>

    .container {
        display: flex;

    }

    .content {
        flex: 1;
        padding: 20px;
    }

</style>
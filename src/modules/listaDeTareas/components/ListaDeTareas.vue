<template>
    <div>
        <h2>Lista de Tareas</h2>
        <input type="text" v-model="nuevaTarea" @keyup.enter="addTarea">
        <ul>
            <li v-for="(tarea, index) in tareas" :key="index">
                {{ tarea }}
                <button @click="borrarTarea">Borrar</button>
            </li>
        </ul>
    </div>
</template>

<script setup>
import {ref} from 'vue';
// Crear lista de tareas
const tareas = ref([]);
const nuevaTarea = ref('');
const addTarea = () => {
    tareas.value.push(nuevaTarea.value);
    nuevaTarea.value = '';
}

// Borrar la tarea
const borrarTarea = (index) => {
    tareas.value.splice(index, 1);
}

</script>

<style></style>
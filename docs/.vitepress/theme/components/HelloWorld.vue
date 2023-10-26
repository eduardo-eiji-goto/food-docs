<script setup>
import { ref } from "vue";

const props = defineProps({
    text: String,
});

const count = ref(0);
</script>

<template>
    <div>
        <h2>{{ text }}</h2>
        <button @click="count = count + 1">Count is: {{ count }}</button>
    </div>
</template>

<style scoped></style>

<script setup>
  defineProps(['title','persons','count'])

</script>

<template>
    <h1>{{ title}}</h1>
    <ul>
        <li v-for="person in persons">
            {{ person.name }}
        </li>
    </ul>
    <h2>{{ count }}</h2>
    <button @click="count++">click +</button>
    <button @click="count--">click -</button>
</template>


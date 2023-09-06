<script setup>
import ChildComponent from "@/components/ChildComponent.vue";
import {reactive, ref} from "vue";

const personLists = reactive([
    {
        name: 'asif',
        age: 30,
        is_active: 1
    },
    {
        name: 'ahmed',
        age: 31,
        is_active: 1
    },
    {
        name: 'ali',
        age: 33,
        is_active: 0
    }
])

const count = ref(0)
</script>

<template>
    <ChildComponent title="Person list" :persons="personLists" :count="count"/>
</template>


<template>
  <HelloWorld :name="name"  :age = "age"/>

<input type="text" v-model="user.name">
<input type="text" v-model="user.age">
</template>

<script setup>
import HelloWorld from '@/components/HelloWorld.vue';

import {reactive} from 'vue';

const user = reactive ( target, {
name: 'NordCoders',
age: 30,
});

const display = () =>{
  console.log(user.name, user.age);
}

display();
</script>

<style scoped>

</style>

<template>
  <HelloWorld :sub-title="subTitle" />

<input type="text" v-model="subTitle">
</template>

<script setup>
import HelloWorld from '@/components/HelloWorld.vue';

const subTitle = "Lorem ipsum";
</script>

<style scoped>

</style>

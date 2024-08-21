<template>
  <div class="app">
    <Vue3Dropzone multiple v-model="files" width="100%" height="400px" imgWidth="150px" imgHeight="150px" showSelectButton :maxFiles="20"
                  :maxFileSize="10" :accept="['.png','.jpg','.jpeg']"></Vue3Dropzone>
  </div>
</template>

<script setup>
import Vue3Dropzone from "./components/Vue3Dropzone.vue";
import {ref} from "vue";

const files = ref([])
</script>

<style lang="scss" scoped></style>

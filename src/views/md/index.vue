<script setup lang="ts">
import { ref } from "vue";
import { MdEditor, MdViewer } from "@/components/Markdown";
import { md } from "./data";

const content = ref(md);
</script>

<template>
  <MdEditor v-model="content"/>
  <MdViewer :content="content"/>
</template>

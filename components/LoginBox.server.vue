<template>
    <div>
    <!-- Hidden input field to hold the extracted token -->
    <input type="hidden" v-model="extractedToken" />
    
    <!-- Display the extracted token (for demonstration) -->
    <p>Extracted Token: {{ extractedToken }}</p>
  </div>
  
</template>

<script setup lang="ts">
import { ref } from 'vue'
const extractedToken = ref("")
async function loadData(){
    extractedToken.value = "value"
  } 
loadData()
</script>

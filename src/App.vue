<script setup>
import Alert from "./components/Alert.vue";

</script>

<template>
  <div class="flex flex-col gap-2 justify-center items-center min-h-screen">
    <Alert type="primary">
      Burası primary alert kutusu
    </Alert>
    <Alert type="warning">
      Burası primary warning kutusu
    </Alert> 
    <Alert type="danger">
      Burası primary danger kutusu
    </Alert> 
    <Alert type="info">
      Burası primary info kutusu
    </Alert> 
  </div>
</template>

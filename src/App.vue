<script setup>
import Alert from "./components/Alert.vue";

</script>

<template>
  <div class="flex justify-center items-center min-h-screen bg-gray-200">
    <div class="w-80 flex flex-col gap-2 bg-white p-2 rounded">
      <h1 class="text-center">Alert Components</h1>
      <hr>
      <Alert type="primary">
        Burası primary alert kutusu Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel, molestiae.
      </Alert>
      <Alert type="warning">
        Burası primary warning kutusu Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel, molestiae.
      </Alert>
      <Alert type="success">
        Burası primary success kutusu Lorem ipsum dolor sit amet consectetur
      </Alert> 
      <Alert type="danger">
        Burası primary danger kutusu Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel, molestiae.
      </Alert> 
      <Alert type="info">
        Burası primary info kutusu
      </Alert> 
    </div>
  </div>
</template>

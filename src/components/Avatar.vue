<template>
    <div>
      <img :src="url" :style="{ width: tamaño + 'px', height: tamaño + 'px' }" alt="Avatar" class="img-fluid" />
    </div>
  </template>
  
  <script>
  export default {
    name:`Avatar`,
    props: {
      url: {
        type: String,
        required: true
      },
      tamaño: {
        type: Number,
        required: true
      }
    }
  };
  </script>
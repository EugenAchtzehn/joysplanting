<template>
  <div class="container py-3">
    <div class="row g-3">
      <div class="col-md-4">
        <div class="content-box p-3">
          <div class="input-group mb-3">
            <button class="btn btn-primary" type="button" @click="increment">Increment</button>
          </div>
          <div>Counter: {{ counter }}</div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="content-box"></div>
      </div>
      <div class="col-md-4">
        <div class="content-box"></div>
      </div>
    </div>
  </div>
</template>
<script setup>
  import { ref } from 'vue';
  const counter = ref(0);

  const increment = () => {
    counter.value++;
  };
</script>

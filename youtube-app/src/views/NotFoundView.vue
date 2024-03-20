<template>
  <div class="wrapper">
    <img class="not-found" alt="img-not-found" src="../assets/404-error.png">
    <span class="text">Sorry, the page is Not Found</span>
  <button class="button" type="button" @click="router.push({ path: '/' })">GO HOME</button>
  </div>
</template>

<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();

</script>

<style scoped>
.wrapper {
  display: flex;
  align-items: center;
  flex-direction: column;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.text {
  font-weight: 700;
  font-size: 1.56rem;
  line-height: 1.4rem;
  margin: 0 0 1.25rem 0;
}

.not-found {
  width: 15.625rem;
  height: 15.625rem;
}

.button {
  padding: 0.625rem;
  color: #8f54c7;
  background-color: #ffffff;
  border: 0.125px solid #8f54c7;
  cursor: pointer;
  font-weight: 500;
}

.button:hover {
  color: #ffffff;
  background-color: #8f54c7;
}
</style>

<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<template>
  <main>
    <section class="container">
      <p class="label">INFO 2500</p>

      <h1>Learning Vue with Vite</h1>

      <p class="name">Created by Jaleigh Bemis</p>

      <p class="description">
        This application was created using Vue 3 and Vite.
        Vite makes it easier to build and organize Vue projects.
      </p>

      <div class="tools">
        <h2>Tools Used</h2>

        <ul>
          <li>Vue 3</li>
          <li>Vite</li>
          <li>CSS</li>
        </ul>
      </div>

      <button @click="count++">
        Button clicked {{ count }} times
      </button>
    </section>
  </main>
</template>

<style scoped>
main {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #20242b;
  font-family: Arial, sans-serif;
  padding: 30px;
}

.container {
  width: 100%;
  max-width: 650px;
  background-color: #2b3038;
  padding: 45px;
  border-radius: 10px;
  color: #f4f4f4;
  border-top: 5px solid #8c9eff;
}

.label {
  margin: 0 0 10px;
  color: #aeb8ff;
  font-size: 14px;
  font-weight: bold;
  letter-spacing: 2px;
}

h1 {
  margin: 0;
  font-size: 36px;
}

.name {
  margin-top: 10px;
  color: #bfc4cc;
}

.description {
  margin-top: 30px;
  line-height: 1.6;
  color: #d6d9de;
}

.tools {
  margin-top: 30px;
}

h2 {
  font-size: 20px;
  color: #aeb8ff;
}

ul {
  padding-left: 20px;
  line-height: 1.8;
}

button {
  margin-top: 20px;
  padding: 11px 18px;
  border: none;
  border-radius: 5px;
  background-color: #8c9eff;
  color: #20242b;
  font-size: 14px;
  font-weight: bold;
  cursor: pointer;
}

button:hover {
  background-color: #aeb8ff;
}
</style>
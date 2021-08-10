<template>
    <div>
    <nav class="lg:block bg-gray-900 bg-opacity-70 z-10">
      <ul class="flex space-x-5 lg:space-x-8 items-center p-4">
        <li class="font-bold text-3xl text-red-600">VueFlix</li>
        <li v-for="link in navLinks" :key="link.name">
          <router-link
            :to="link.href"
            class="font-bold text-sm lg:text-base text-white hover:text-app-green-1 transition ease-in-out duration-300"
            >{{ link.name }}</router-link
          >
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";

export default {
  components: {
    Header
  
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

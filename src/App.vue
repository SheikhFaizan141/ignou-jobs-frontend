<script setup>
import { RouterLink, RouterView, useRoute, useRouter } from 'vue-router'
import AppFooter from '@/components/AppFooter.vue'
const router = useRouter();
const route = useRoute();
console.log(route.meta);

</script>

<template>
  <header class="flex items-center  p-2 border border-b-gray-200">
    <!-- <img alt="Vue logo" class="logo" src="@/" width="125" height="125" /> -->
    <h1 class="text-4xl  basis-1/4">
      <RouterLink to="/">Ignou Jobs</RouterLink>
    </h1>

    <div class="basis-3/4 ">
      <nav class="flex justify-end">
        <!-- <RouterLink to="/">Home</RouterLink> -->
        <RouterLink to="/signin">Sign in</RouterLink>
        <div class="h-divider h-5 border-r border-r-black"></div>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />



  <AppFooter />
</template>

<style scoped></style>

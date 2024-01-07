<script setup>
import { ref } from 'vue';
import { useRoute } from 'vue-router';

const email = ref('');
const password = ref('');


const submit = () => {
    console.log(email);
    console.log(password);
}

const route = useRoute();

console.log(route.meta);

</script>

<template>
    <main class="flex justify-center items-center">
        <div class="flex  flex-col w-1/4 border border-black p-3 rounded shadow shadow-gray-500">
            <h1 class="text-2xl mb-3 font-bold">Sign In</h1>
            <form>
                <div class="mb-3 ">
                    <label for="email" class="block">Enter Email</label>
                    <input
                    id="email"
                    type="email"
                    class="block w-full"
                    label="Email"
                    v-model="email"
                    placeholder="enter email"
                    />
                </div>

                <div class="mb-3">
                    <label for="password" class="block">Enter Password</label>
                    <input
                    id="password"
                    type="password"
                    class="block w-full"
                    label="Password"
                    v-model="password"
                    placeholder="enter password"
                    />
                </div>

                <div class="mb-3">
                    <label for="">Remember me</label>
                    <input
                    type="checkbox"
                    class="tw-mb-4"
                    label="Remember me"
                    />
                </div>
                <button
                    class="focus:outline-none text-white bg-green-700 hover:bg-green-800 focus:ring-4 focus:ring-green-300 font-medium rounded-lg text-sm px-5 py-2.5 me-2 mb-2 dark:bg-green-600 dark:hover:bg-green-700 dark:focus:ring-green-800"
                    color="primary"
                    @click="submit"
                >Sign in</button>
            </form>
        </div>
    </main>
</template>

<style >
html {
    height: 100dvh;
}

body { 
    /* height: 100%; */
    /* background-color: orange; */
}

main {
    height: 100%;
    background-color: aqua;
}

</style>
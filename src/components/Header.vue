<script setup lang="ts">
import { useUserStore } from "../stores/user";
import {useRouter} from "vue-router";


const userStore = useUserStore();
const router = useRouter();

const logout = () => {
    userStore.logout();
    router.push('/');
};

</script>

<template>
    <div class="py-4 px-6 bg-gray-800 shadow-md flex justify-between items-center">
        <h1>Chat IA</h1>
        <button class="text-gray-400 hover:text-white" @click="logout">Logout</button>
    </div>
</template>
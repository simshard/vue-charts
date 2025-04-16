<template>
    <div class="h-screen text-white dark:bg-gray-900">
        <Navbar />
        <h1 class="text-3xl text-indigo-400">Home</h1>
    </div>
</template>

<script>
import Navbar from '../Shared/Navbar.vue';
export default {
    components: { Navbar },
};
</script>

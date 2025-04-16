<template>
    <div class="h-screen text-white dark:bg-gray-900">
        <Navbar />
        <h1 class="text-3xl text-indigo-400">Users</h1>
        <div style="margin-top: 1200px" class="p-8 text-gray-500">
            Current time : {{ time }}
        <Link href="/users" preserve-scroll>refresh</Link>
        </div>
    </div>
</template>
<script>
import Navbar from '../Shared/Navbar.vue';
import { Link } from '@inertiajs/vue3';
export default {
    // eslint-disable-next-line vue/no-reserved-component-names
    components: { Navbar, Link },
    props: {
        time: String,
    },
};
</script>

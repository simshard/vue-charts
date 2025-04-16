<template>
    <nav class="flex justify-center">
        <ul class="flex flex-row space-x-4">
            <li>
                <Link
                    href="/"
                    :class="{ 'italic underline': $page.url === '/' }"
                    >Home</Link
                >
            </li>
            <li>
                <Link
                    href="/settings"
                    :class="{
                        'italic underline': $page.url.startsWith('/settings'),
                    }"
                    >Settings</Link
                >
            </li>
            <li>
                <Link
                    href="/users"
                    :class="{
                        'italic underline': $page.url.startsWith('/users'),
                    }"
                    >Users</Link
                >
            </li>
            <li>
                <Link href="/logout" method="post" as="button">Logout</Link>
            </li>
        </ul>
    </nav>
</template>

<script>
import { Link } from '@inertiajs/vue3';
export default {
    // eslint-disable-next-line vue/no-reserved-component-names
    components: { Link },
};
</script>

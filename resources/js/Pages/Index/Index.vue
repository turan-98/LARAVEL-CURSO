<template>
    <div>Index</div>
    <Link rel="stylesheet" href="/hello">Show Page</Link>
    <div>
        The message is {{message}}
    </div>
</template>
<script setup>
import {Link}  from '@inertiajs/vue3'
defineProps({
    message:String
})
</script>
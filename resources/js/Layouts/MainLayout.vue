<template>
   <Link href="/">Main page</Link>
   <Link href="/hello">Show page</Link>
   <slot>Default</slot>
   <div>The page with timer {{ timer }}</div>
</template>

<script setup>
import {Link} from '@inertiajs/vue3'
import {ref} from 'vue'

const timer = ref(0)
setInterval(() => timer.value++, 1000)
</script>

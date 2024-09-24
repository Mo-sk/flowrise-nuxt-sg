<script setup lang="ts">
defineProps<{
    as?: string
}>()
</script>

<template>
    <Component
        :is="as || 'section'"
        class="px-4 py-10 md:px-6 md:py-14 lg:py-16"
    >
        <div class="mx-auto max-w-6xl w-full">
            <slot />
        </div>
    </Component>
</template>
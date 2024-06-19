<template>
    <div class="flex flex-col items-start justify-center px-3 py-3.5 text-sm text-gray-600">
        <h5 class="font-semibold">{{ props.role }}</h5>
        <span class="font-normal">{{ props.summary }}</span>
    </div>
</template>

<script setup>
const props = defineProps({
    role: { type: String, required: true },
    summary: { type: String, required: true }
});
</script>
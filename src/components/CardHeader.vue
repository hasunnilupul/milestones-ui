<template>
    <div class="flex items-center justify-start p-3 w-full border-b border-gray-200 text-base text-gray-600">
        <h5 class="font-semibold">{{ props.org }}</h5>
        <span class="ml-2 font-normal">{{ props.duration }}</span>
    </div>
</template>

<script setup>
const props = defineProps({
    org: { type: String, default: "" },
    duration: { type: String, default: "" }
});
</script>
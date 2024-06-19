<template>
    <div
        class="flex flex-row items-center justify-start px-3 py-2 w-fit bg-red-100 rounded-md border-l-4 border-red-600 text-red-500">
        <h5 class="font-bold">{{ props.title }}</h5>
        <span class="ml-2 font-normal">{{ props.message }}</span>
    </div>
</template>

<script setup>
const props = defineProps({
    title: { type: String, required: true },
    message: { type: String, default: "" },
});
</script>
<template>
    <div class="flex flex-col items-start justify-start w-full bg-white rounded-md">
        <!-- card header -->
        <CardHeader v-if="showHeader" :org="props.org" :duration="props.duration" />

        <!-- card body -->
        <CardBody :role="props.role" :summary="props.summary" />
    </div>
</template>

<script setup>
import { computed } from "vue";

import CardHeader from "@/components/CardHeader.vue";
import CardBody from "@/components/CardBody.vue";

const props = defineProps({
    org: { type: String, default: "" },
    duration: { type: String, default: "" },
    role: { type: String, required: true },
    summary: { type: String, required: true }
});

const showHeader = computed(() => props.org !== "" && props.duration !== "")
</script>
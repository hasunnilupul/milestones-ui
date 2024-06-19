<template>
    <div class="flex flex-row items-start justify-between">
        <div class="grow-0 mx-4">
            <span class="block rounded-full w-2 h-2 mt-5 blur-[0.75px] bg-orange-500" />
        </div>
        <div class="grow flex-col space-y-5">
            <slot></slot>
        </div>
    </div>
</template>
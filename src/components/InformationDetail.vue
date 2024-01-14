<template>
    <div class="w-full">
        <div class="flex flex-row flex-nowrap items-center gap-x-4 mb-2">
            <div class="w-[32px] h-[32px] flex flex-row items-center justify-center">
                <img src="@/assets/icons/dark-telephone.png">
            </div>
            <div class="flex-grow">
                <p class="mb-0 text-base font-medium leading-[18.96px] uppercase text-[#006FEB]">{{ label }}</p>
            </div>
        </div>
        <div class="flex flex-row flex-nowrap items-center gap-x-4">
            <div class="w-[32px] flex flex-row"></div>
            <div class="flex-grow text-[18px] leading-[21.33px]">
                <slot>
                    <p class="mb-0">
                        {{  content }}
                    </p>
                </slot>
            </div>
        </div>
    </div>
</template>
<script setup>
    import { defineProps } from "vue";

    defineProps({
        label: {
            type: String,
            default: null
        },
        content: {
            type: String,
            default: null
        }
    })
</script>
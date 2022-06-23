<template>
    <div class="flex p-2 rounded w-full" :class="alertStyle">
      <slot></slot>
    </div>
</template>
<script setup>
import { computed } from '@vue/reactivity';

    const props = defineProps({
        type:{
            default:"primary",
            type: String
        }
    })

    const alertStyle = computed(() => {
        return [
            {'primary':props.type === "primary"},
            {'warning':props.type === "warning"},
            {'danger':props.type === "danger"},
            {'info':props.type === "info"},
        ]
    })
</script>

<style scoped>
    .primary{
        @apply bg-blue-200 border border-blue-500 text-blue-700
    }
    .warning{
        @apply bg-yellow-200 border border-yellow-500 text-yellow-700
    }
    .danger{
        @apply bg-red-200 border border-red-500 text-red-700
    }
    .info{
        @apply bg-gray-200 border border-gray-500 text-gray-700
    }
</style>
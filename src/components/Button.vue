<template>
    <button @click="onClick()" :style="{ background: color }" class="btn">{{ text }}</button>
</template> 

<script>
export default {
    name: 'Button',
    props: {
        text: {
            type: String,
            default: "button",
            required: true
        },
        color: {
            type: String,
            default: "blue",
            required: true
        }
    },
    methods: {
        onClick() {
            this.$emit('btn-click')
        },
    }
}
</script>

<style>
</style>

<template>
    <button :style="{background: color}" class="btn" >{{title}}</button>
</template> 

<script>
export default {
    name: 'Button',
    props: {
        title: {
            type: String,
            default: "button",
            required: true
        },
        color: {
            type: String,
            default: "blue",
            required: true
        }
    }
}
</script>

<style>

</style>

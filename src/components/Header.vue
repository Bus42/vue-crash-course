<template>
    <header>
        <h1>{{ title }}</h1>
        <Button title="Add Task" color="green" />
    </header>
</template>

<script>
import Button from "./Button.vue";
export default {
    name: 'Header',
    props: {
        title: {
            type: String,
            default: "Title",
            required: true
        }
    },
    components: {
        Button
    }
}
</script>

<style scoped >
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}
</style>

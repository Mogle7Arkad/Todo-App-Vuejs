<script>
export default {
    name: 'Task',
    props: {
        task: Object
    }
}
</script>

<template>
    <h5>{{ task.text }}</h5>
</template>
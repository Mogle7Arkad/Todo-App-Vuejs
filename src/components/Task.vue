<script>
export default {
    name: 'Task',
    props: {
        task: Object
    }
}
</script>

<template>
<div class="task">
    <h5>{{ task.text }}</h5>
    <p>{{ task.day }}</p>
</div>
</template>

<style scoped>
.task{
    background: #f4f4f4;
    margin: 5px;
    padding: 10px 20px;
    cursor: pointer;
}

.task.reminder {
    border-left: 5px solid green;
}

.task h5 {
    display: flex;
    align-items: center;
    justify-content: space-between;
}
</style>
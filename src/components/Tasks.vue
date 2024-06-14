<script>
export default {
    name: 'Tasks',
    props:{
        tasks: Array
    }
}
</script>

<template>
    <div :key="task.id" v-for="task in tasks">
        <h5>{{ task.text }}</h5>
    </div>
</template>
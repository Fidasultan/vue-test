<template>
    <div class="container">
        <div class="jumbotron">
            <h1>Task Detail</h1>
            <p>
                <b>Task</b>: {{task.task}}
            </p>
            <p>
                <b>Assignee:</b> {{task.assignee}}
            </p>
            <p>
            <b>Status:</b> {{task.status}}
            </p>
        </div>
    </div>
</template>

<script>
    const task = JSON.parse(localStorage.getItem("task"))
    console.log(task);
    export default {
        name: 'Detail',
        data() {
            return {
                task: JSON.parse(localStorage.getItem("task"))
            }
    }
    }
</script>
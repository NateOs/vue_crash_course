<template>
  <div class="task">
    <div class="task-title">
      <h3>
        {{ task.title }}
      </h3>
      <i class="fas fa-times"></i>
    </div>

    <p>{{ task.description }}</p>
  </div>
</template>
<script>
export default {
  name: "TaskListComponent",
  props: {
    task: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped>
.fas {
  color: red;
}
.task {
  background: #f4f4f4;
  margin: 5px;
  padding: 10px 20px;
  cursor: pointer;
}
.task-title {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>

<template>
  <div class="task">
    <h3>{{ task.title }}</h3>
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
.task {
  background: #f4f4f4;
  margin: 5px;
  padding: 10px 20px;
  cursor: pointer;
}
</style>

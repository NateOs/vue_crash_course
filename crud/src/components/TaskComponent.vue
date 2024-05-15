<template>
  <div :key="task.id" v-for="task in tasks">
    
    <TaskListComponent :task="task" key="task.id" />
  </div>
</template>

<script>
import TaskListComponent from "./TaskListComponent.vue";

export default {
  name: "TaskComponent",
  components: {
    TaskListComponent,
  },
  props: {
    tasks: Array,
  },
};
</script>

<style scoped></style>

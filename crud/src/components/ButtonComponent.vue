<template>
  <button :style="{ background: color }" class="btn" @click="handleClick">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "ButtonComponent",
  props: {
    text: String,
    color: String,
  },
  methods: {
    handleClick() {
      console.log("clicked");
    },
  },
};
</script>

<style scoped></style>

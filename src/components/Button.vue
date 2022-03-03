<template>
  <button @click="onClickHandler()" :style="{ background: color }" class="btn">
    {{ text }}
  </button>
</template>
<script>
export default {
  name: "Button",
  props: {
    text: String,
    color: String,
  },
  methods: {
    onClickHandler() {
      this.$emit("btn-click");
    },
  },
};
</script>

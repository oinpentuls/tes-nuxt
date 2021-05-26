<template>
  <button
    :class="`bg-blue-100 py-4 btn-start rounded ${className}`"
    @click="toggleValue"
  >
    {{ label }}
  </button>
</template>

<script>
export default {
  props: {
    label: {
      type: String,
      default: "",
    },
    className: {
      type: String,
      default: "",
    },
    toggle: {
      type: Boolean,
      default: false,
    },
  },
  data() {
    return {}
  },
  methods: {
    toggleValue() {
      this.$emit('click', this.toggle)
    }
  }
};
</script>
<style>
.btn-start {
  /* padding: 0.8rem 1.7rem; */
  background: #2b80a3;
  color: white;
  text-align: center;
  font-weight: bold;
  border: 1px solid #2b80a3;
}

.btn-start:hover {
  transition: ease-in 0.1s;
  background: white;
  color: #2b80a3;
  border: 1px solid #2b80a3;
}
</style>
